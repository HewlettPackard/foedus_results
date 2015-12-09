FOEDUS experiments package for MCSg Artifact Evaluation (AE)
========
This folder contains a fork of FOEDUS codebase we used for the MCSg paper.
It is a tar-ed git repo image of our internal git fork.

Contents of this folder
--------

1. [foedus_internal.tar.gz](foedus_internal.tar.gz) : The tar-ed repo.
2. [README.markdown](README.markdown) : This document.


Prerequisite
--------
To shorten this document, we assume you have already applied the general environmental
configuration for FOEDUS. If not, see:
  https://github.com/hkimura/foedus_code/tree/master/foedus-core

Especially, please make sure "ctest -R check_env" passes all environmental tests
(currently there are 16 of them) and also you have a sufficient number of
non-transparent hugepages allocated. We note that the most common pitfall in
setting up FOEDUS is hugepage-allocation for shared-memory use, which requires
configuring ulimit/sysctl etc correctly.


Untar/Compile
--------
To compile this code, simply:

    [kimurhid@hkimura-z820 20151209_mcsg_code_repo]$ tar -xf foedus_internal.tar.gz 
    [kimurhid@hkimura-z820 20151209_mcsg_code_repo]$ cd foedus_code_clone/
    [kimurhid@hkimura-z820 foedus_code_clone]$ git checkout mcsg_exp 
    Switched to branch 'mcsg_exp'
    Your branch is up-to-date with 'origin/mcsg_exp'.
    [kimurhid@hkimura-z820 foedus_code_clone]$ cd release/
    [kimurhid@hkimura-z820 release]$ cmake ../ -DCMAKE_BUILD_TYPE=Release
    <....>
    [kimurhid@hkimura-z820 release]$ make -j
    <....>

Running the experiment
--------
Go down to the TPC-C folder:

    [kimurhid@hkimura-z820 release]$ cd experiments-core/src/foedus/tpcc/
    
Then, run the following.
    
    # NOTE: You must configure the parameters below depending on the size of your machine.
    # We recommend :
    #   thread_per_node = #-of-cores-per-socket - 1 or 2 (leave one or two core for OS! Do not count HTT-ed cores)
    #   numa_nodes = #-of-sockets
    # Also, please note that even TATAS is as fast as MCS/MCSg with a small number of threads.
    # Please run the experiments on the largest machine you have.
    for rep in 0 1 2 3 4 5 6 7 8 9
    do
        rm -rf /dev/shm/foedus_tpcc/
        rm -rf /tmp/libfoedus.*
        env CPUPROFILE_FREQUENCY=1 ./tpcc -warehouses=1 -take_snapshot=false -fork_workers=false -nvm_folder=/dev/shm -high_priority=false -null_log_device=true -loggers_per_node=1 -thread_per_node=8 -numa_nodes=2 -log_buffer_mb=128 -volatile_pool_size=2 -snapshot_pool_size=1 -reducer_buffer_size=1 -duration_micro=10000000 &> "result$rep.log"
    done

To collect the result,

    grep "final result" result*

whose output would look like:

    result0.log:I1209 11:28:34.959004 24520 tpcc_driver.cpp:638] final result:<total_result><duration_sec_>10.0001</duration_sec_><worker_count_>16</worker_count_><processed_>14738844</processed_><MTPS>1.47386</MTPS><user_requested_aborts_>0</user_requested_aborts_><race_aborts_>27754</race_aborts_><largereadset_aborts_>0</largereadset_aborts_><unexpected_aborts_>0</unexpected_aborts_><snapshot_cache_hits_>0</snapshot_cache_hits_><snapshot_cache_misses_>0</snapshot_cache_misses_></total_result>

Here, the content of "MTPS" element is the million transactions per second in the paper.
A bit of regex and pasting to a spreadsheet program (e.g., libreoffice) would give
you the average and stdev.

Switching the implementation
--------
As in the paper, we evaluate three lock implementations.
Unfortunately, we switch these implementations at compile time, not as a runtime parameter.

Open the following file:

    [kimurhid@hkimura-z820 tpcc]$ emacs -nw ../../../../../foedus-core/src/foedus/thread/thread_pimpl.cpp

At Line 55, find the following:
    
    /** Just for MCSg paper. */
    constexpr bool kDebugUseTatas = true;
    constexpr bool kDebugUseMcsg = true;

Set the following values for the three alternatives.

1. MCSg: kDebugUseMcsg = true, kDebugUseTatas = false
2. MCS: kDebugUseMcsg = false, kDebugUseTatas = false
3. TATAS: kDebugUseMcsg = false, kDebugUseTatas = true

Finally, do not forget to re-compile *each time* after configuring them.

    make -j

That is it. Thank you very much.
If you hit any issue, please do not hesitate to contact us (probably via the program chair).

Tianzheng, Milind, and Hideaki. Dec'15.


First perforamnce test on smaug-3.

Script (16 workers per socket):

    warehouses=256
    loggers_per_node=2
    volatile_pool_size=32
    snapshot_pool_size=2
    reducer_buffer_size=1
    duration_micro=10000000
    thread_per_node=16
    numa_nodes=16
    log_buffer_mb=1024
    machine_name="DragonHawk"
    machine_shortname="dh"
    . run_common.sh


Results:

    result_tpcc_dh.n0 16.9593
    result_tpcc_dh.n0 16.2184
    result_tpcc_dh.n0 17.426
    result_tpcc_dh.n1 15.5844
    result_tpcc_dh.n1 16.4588
    result_tpcc_dh.n1 15.9509
    result_tpcc_dh.n2 16.5192
    result_tpcc_dh.n2 15.9432
    result_tpcc_dh.n2 17.1009
    result_tpcc_dh.n3 15.7612
    result_tpcc_dh.n3 16.845
    result_tpcc_dh.n3 15.4215
    result_tpcc_dh.n4 16.0529
    result_tpcc_dh.n4 15.369
    result_tpcc_dh.n4 15.9655
    result_tpcc_dh.n5 15.5002
    result_tpcc_dh.n5 15.808
    result_tpcc_dh.n5 15.8227
    result_tpcc_dh.n6 16.2303
    result_tpcc_dh.n6 15.1881
    result_tpcc_dh.n6 15.9487
    result_tpcc_dh.n7 15.5843
    result_tpcc_dh.n7 16.0715
    result_tpcc_dh.n7 15.4087
    result_tpcc_dh.n8 15.8338
    result_tpcc_dh.n8 15.405
    result_tpcc_dh.n8 16.0541
    result_tpcc_dh.n9 15.3682
    result_tpcc_dh.n9 16.2401
    result_tpcc_dh.n9 14.9401
    result_tpcc_dh.n10 16.1243
    result_tpcc_dh.n10 15.4631
    result_tpcc_dh.n10 16.0499

17 MTPS!


Performance regression test on puff (smaug-3) after the bug fix on write-set sorting.
The sorting is now slightly more costly, so we wanted to confirm its performance effect.

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


Results (upto n=3):

    result_tpcc_dh.n0.r0 16.8803
    result_tpcc_dh.n0.r1 16.8356
    result_tpcc_dh.n0.r2 16.9626
    result_tpcc_dh.n1.r0 16.5347
    result_tpcc_dh.n1.r1 16.5008
    result_tpcc_dh.n1.r2 16.5375
    result_tpcc_dh.n2.r0 16.4189
    result_tpcc_dh.n2.r1 16.3027
    result_tpcc_dh.n2.r2 16.2977

Okay, no statistically significant difference from 20150915.

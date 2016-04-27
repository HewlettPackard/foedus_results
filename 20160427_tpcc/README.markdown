
Performance regression test on smaug-1 after merging MOCC.
null_log_device is true.

    result_tpcc_dh.n0.r1 11.4421
    result_tpcc_dh.n0.r2 11.5011
    result_tpcc_dh.n1.r0 11.057
    result_tpcc_dh.n1.r1 11.0166
    result_tpcc_dh.n1.r2 11.1256
    result_tpcc_dh.n2.r0 10.995
    result_tpcc_dh.n2.r1 11.1843
    result_tpcc_dh.n2.r2 11.0243
    result_tpcc_dh.n3.r0 11.0272
    result_tpcc_dh.n3.r1 10.9246
    result_tpcc_dh.n3.r2 10.596
    result_tpcc_dh.n4.r0 10.8269
    result_tpcc_dh.n4.r1 10.7291
    result_tpcc_dh.n4.r2 10.8121
    result_tpcc_dh.n5.r0 10.5358
    result_tpcc_dh.n5.r1 10.6791
    result_tpcc_dh.n5.r2 10.7251
    result_tpcc_dh.n6.r0 10.6619
    result_tpcc_dh.n6.r1 10.6053
    result_tpcc_dh.n6.r2 10.615
    result_tpcc_dh.n7.r0 10.648
    result_tpcc_dh.n7.r1 10.4739
    result_tpcc_dh.n7.r2 10.5251
    result_tpcc_dh.n8.r0 10.4106

Not much difference, but CPU profile indicates higher sorting cost because now we do it twice (CLL and read/write set).
Just a few percent, but we might want to merge them in future.


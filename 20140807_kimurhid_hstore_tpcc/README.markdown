Contact: kimurhid
Experiment: foedus/tpcc/hstore
Date: 2014/08/08

Version
-------
H-Store from repository latest as of 08/01

Environment
-------
3 Environments


Z820 FOEDUS TPC-C Results
-------
See the run_hstore_z820.sh.
Result summary:

    [kimurhid@hkimura-z820 20140807_kimurhid_hstore_tpcc]$ grep Throughput *
    hstore_tpcc_z820.n0.r0.log:     [java] Throughput:     53707.80 txn/s [min:47631.80 / max:60970.60 / stdev:5456.08]
    hstore_tpcc_z820.n0.r1.log:     [java] Throughput:     58164.07 txn/s [min:52600.90 / max:67269.80 / stdev:5736.12]
    hstore_tpcc_z820.n0.r2.log:     [java] Throughput:     71583.68 txn/s [min:66788.60 / max:74829.10 / stdev:3039.74]
    hstore_tpcc_z820.n10.r0.log:     [java] Throughput:     3774.55 txn/s [min:2980.10 / max:5581.90 / stdev:1005.33]
    hstore_tpcc_z820.n10.r1.log:     [java] Throughput:     3847.93 txn/s [min:3251.80 / max:4689.20 / stdev:573.78]
    hstore_tpcc_z820.n10.r2.log:     [java] Throughput:     3835.13 txn/s [min:2477.50 / max:5072.70 / stdev:943.60]
    hstore_tpcc_z820.n1.r0.log:     [java] Throughput:     40308.47 txn/s [min:32656.30 / max:47944.50 / stdev:4841.34]
    hstore_tpcc_z820.n1.r1.log:     [java] Throughput:     33254.23 txn/s [min:28143.20 / max:37503.30 / stdev:3398.53]
    hstore_tpcc_z820.n1.r2.log:     [java] Throughput:     33847.88 txn/s [min:30611.10 / max:38999.50 / stdev:3202.24]
    hstore_tpcc_z820.n2.r0.log:     [java] Throughput:     29959.85 txn/s [min:27533.20 / max:34135.30 / stdev:2410.63]
    hstore_tpcc_z820.n2.r1.log:     [java] Throughput:     28771.32 txn/s [min:26319.30 / max:30423.20 / stdev:1602.30]
    hstore_tpcc_z820.n2.r2.log:     [java] Throughput:     27167.23 txn/s [min:24236.70 / max:28718.90 / stdev:1636.71]
    hstore_tpcc_z820.n3.r0.log:     [java] Throughput:     21139.45 txn/s [min:18355.40 / max:23135.80 / stdev:1874.99]
    hstore_tpcc_z820.n3.r1.log:     [java] Throughput:     22216.58 txn/s [min:19377.30 / max:27225.30 / stdev:2702.37]
    hstore_tpcc_z820.n3.r2.log:     [java] Throughput:     19112.45 txn/s [min:16154.30 / max:25163.70 / stdev:3519.60]
    hstore_tpcc_z820.n4.r0.log:     [java] Throughput:     14388.88 txn/s [min:11948.00 / max:18236.80 / stdev:2260.12]
    hstore_tpcc_z820.n4.r1.log:     [java] Throughput:     14509.75 txn/s [min:12179.60 / max:17647.80 / stdev:2289.94]
    hstore_tpcc_z820.n4.r2.log:     [java] Throughput:     14934.85 txn/s [min:12413.20 / max:18315.70 / stdev:2059.12]
    hstore_tpcc_z820.n5.r0.log:     [java] Throughput:     10967.97 txn/s [min:9536.70 / max:13874.00 / stdev:1534.01]
    hstore_tpcc_z820.n5.r1.log:     [java] Throughput:     11805.95 txn/s [min:9382.70 / max:14703.70 / stdev:2089.07]
    hstore_tpcc_z820.n5.r2.log:     [java] Throughput:     9902.43 txn/s [min:8794.60 / max:11648.70 / stdev:1072.93]
    hstore_tpcc_z820.n6.r0.log:     [java] Throughput:     7506.32 txn/s [min:5047.10 / max:9836.00 / stdev:1545.06]
    hstore_tpcc_z820.n6.r1.log:     [java] Throughput:     8016.83 txn/s [min:6333.20 / max:10086.60 / stdev:1486.44]
    hstore_tpcc_z820.n6.r2.log:     [java] Throughput:     7351.68 txn/s [min:5907.40 / max:8086.60 / stdev:864.19]
    hstore_tpcc_z820.n7.r0.log:     [java] Throughput:     5545.03 txn/s [min:4686.00 / max:7288.60 / stdev:971.00]
    hstore_tpcc_z820.n7.r1.log:     [java] Throughput:     5825.07 txn/s [min:5189.20 / max:6819.50 / stdev:600.91]
    hstore_tpcc_z820.n7.r2.log:     [java] Throughput:     5699.92 txn/s [min:4301.10 / max:7488.70 / stdev:1044.68]
    hstore_tpcc_z820.n8.r0.log:     [java] Throughput:     5058.23 txn/s [min:3833.80 / max:6773.30 / stdev:961.33]
    hstore_tpcc_z820.n8.r1.log:     [java] Throughput:     4854.35 txn/s [min:3767.80 / max:5972.40 / stdev:774.33]
    hstore_tpcc_z820.n8.r2.log:     [java] Throughput:     5245.87 txn/s [min:3890.30 / max:6657.50 / stdev:973.90]
    hstore_tpcc_z820.n9.r0.log:     [java] Throughput:     4493.85 txn/s [min:3704.60 / max:5637.10 / stdev:734.84]
    hstore_tpcc_z820.n9.r1.log:     [java] Throughput:     5047.90 txn/s [min:4578.20 / max:6205.30 / stdev:620.27]
    hstore_tpcc_z820.n9.r2.log:     [java] Throughput:     4862.73 txn/s [min:3930.30 / max:5861.10 / stdev:759.96]


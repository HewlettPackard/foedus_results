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


DL580 Results
--------

hstore_tpcc_dl580.n0.r0.log:     [java] Throughput:     128462.17 txn/s [min:77289.70 / max:214511.80 / stdev:46542.43]
hstore_tpcc_dl580.n0.r1.log:     [java] Throughput:     113280.70 txn/s [min:75734.90 / max:138401.00 / stdev:21015.97]
hstore_tpcc_dl580.n0.r2.log:     [java] Throughput:     125652.32 txn/s [min:94375.90 / max:140959.70 / stdev:16545.03]
hstore_tpcc_dl580.n10.r0.log:     [java] Throughput:     919.30 txn/s [min:637.10 / max:1347.30 / stdev:260.96]
hstore_tpcc_dl580.n10.r1.log:     [java] Throughput:     2112.65 txn/s [min:1484.60 / max:2968.80 / stdev:571.07]
hstore_tpcc_dl580.n10.r2.log:     [java] Throughput:     1457.32 txn/s [min:842.90 / max:2527.10 / stdev:598.72]
hstore_tpcc_dl580.n1.r0.log:     [java] Throughput:     61112.52 txn/s [min:19060.40 / max:146094.70 / stdev:45467.18]
hstore_tpcc_dl580.n1.r1.log:     [java] Throughput:     53010.05 txn/s [min:25175.80 / max:135035.60 / stdev:40870.70]
hstore_tpcc_dl580.n1.r2.log:     [java] Throughput:     64188.15 txn/s [min:45134.20 / max:75843.80 / stdev:12794.04]
hstore_tpcc_dl580.n2.r0.log:     [java] Throughput:     32448.03 txn/s [min:18440.20 / max:48960.60 / stdev:9942.02]
hstore_tpcc_dl580.n2.r1.log:     [java] Throughput:     41086.57 txn/s [min:25855.00 / max:70110.90 / stdev:15651.77]
hstore_tpcc_dl580.n2.r2.log:     [java] Throughput:     46827.02 txn/s [min:26164.00 / max:72887.40 / stdev:17336.22]
hstore_tpcc_dl580.n3.r0.log:     [java] Throughput:     22865.08 txn/s [min:16338.90 / max:35618.90 / stdev:7080.47]
hstore_tpcc_dl580.n3.r1.log:     [java] Throughput:     30115.48 txn/s [min:17113.20 / max:40932.10 / stdev:9884.03]
hstore_tpcc_dl580.n3.r2.log:     [java] Throughput:     26302.57 txn/s [min:19793.60 / max:40421.30 / stdev:7793.68]
hstore_tpcc_dl580.n4.r0.log:     [java] Throughput:     18468.73 txn/s [min:14157.30 / max:23774.70 / stdev:4119.76]
hstore_tpcc_dl580.n4.r1.log:     [java] Throughput:     14082.55 txn/s [min:10104.10 / max:20875.10 / stdev:3698.56]
hstore_tpcc_dl580.n4.r2.log:     [java] Throughput:     17894.97 txn/s [min:11695.60 / max:24968.40 / stdev:4652.87]
hstore_tpcc_dl580.n5.r0.log:     [java] Throughput:     10341.95 txn/s [min:2479.70 / max:13690.70 / stdev:4292.68]
hstore_tpcc_dl580.n5.r1.log:     [java] Throughput:     14363.17 txn/s [min:7954.30 / max:20635.80 / stdev:4581.97]
hstore_tpcc_dl580.n5.r2.log:     [java] Throughput:     8810.45 txn/s [min:5311.00 / max:12953.90 / stdev:3187.84]
hstore_tpcc_dl580.n6.r0.log:     [java] Throughput:     5710.08 txn/s [min:2106.10 / max:9279.70 / stdev:2619.88]
hstore_tpcc_dl580.n6.r1.log:     [java] Throughput:     7925.08 txn/s [min:5496.30 / max:9793.30 / stdev:1491.75]
hstore_tpcc_dl580.n6.r2.log:     [java] Throughput:     8271.68 txn/s [min:5483.90 / max:10733.90 / stdev:2016.92]
hstore_tpcc_dl580.n7.r0.log:     [java] Throughput:     5998.92 txn/s [min:2774.80 / max:8554.60 / stdev:1981.53]
hstore_tpcc_dl580.n7.r1.log:     [java] Throughput:     945.98 txn/s [min:569.20 / max:2606.40 / stdev:814.03]
hstore_tpcc_dl580.n7.r2.log:     [java] Throughput:     4926.43 txn/s [min:1118.60 / max:6511.00 / stdev:1940.16]
hstore_tpcc_dl580.n8.r0.log:     [java] Throughput:     3715.10 txn/s [min:2149.30 / max:5283.00 / stdev:1172.77]
hstore_tpcc_dl580.n8.r1.log:     [java] Throughput:     3371.90 txn/s [min:1430.60 / max:5162.80 / stdev:1355.01]
hstore_tpcc_dl580.n8.r2.log:     [java] Throughput:     3160.25 txn/s [min:1673.50 / max:4775.30 / stdev:1294.21]
hstore_tpcc_dl580.n9.r0.log:     [java] Throughput:     1475.02 txn/s [min:714.80 / max:2850.60 / stdev:746.00]
hstore_tpcc_dl580.n9.r1.log:     [java] Throughput:     2199.50 txn/s [min:518.80 / max:3138.50 / stdev:981.17]
hstore_tpcc_dl580.n9.r2.log:     [java] Throughput:     2122.97 txn/s [min:892.20 / max:3012.90 / stdev:717.40]



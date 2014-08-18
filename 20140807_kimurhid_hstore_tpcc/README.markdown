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

    

DragonHawk Results
--------

    hstore_tpcc_dh.n0.r0.log:     [java] Throughput:     104133.43 txn/s [min:27160.60 / max:175577.20 / stdev:53926.01]
    hstore_tpcc_dh.n0.r0.log:     [java]               Delivery:    312726 (  5.0%)         0 (  0.0%)   5212.10 txn/s   6296.12 ms
    hstore_tpcc_dh.n0.r0.log:     [java]              New Order:   2811888 ( 45.0%)         0 (  0.0%)  46864.80 txn/s   6286.94 ms
    hstore_tpcc_dh.n0.r0.log:     [java]            Stock Level:    187098 (  3.0%)         0 (  0.0%)   3118.30 txn/s   6285.12 ms
    hstore_tpcc_dh.n0.r0.log:     [java]                Payment:   2685421 ( 43.0%)         0 (  0.0%)  44757.02 txn/s   6292.94 ms
    hstore_tpcc_dh.n0.r0.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n0.r0.log:     [java]           Order Status:    250873 (  4.0%)         0 (  0.0%)   4181.22 txn/s   6280.93 ms
    hstore_tpcc_dh.n10.r1.log:     [java] Throughput:     2235.08 txn/s [min:1304.30 / max:4272.50 / stdev:1110.65]
    hstore_tpcc_dh.n10.r1.log:     [java]               Delivery:     32795 ( 24.5%)         0 (  0.0%)    546.58 txn/s   8720.98 ms
    hstore_tpcc_dh.n10.r1.log:     [java]              New Order:      3508 (  2.6%)       159 (  4.5%)     58.47 txn/s  10540.59 ms
    hstore_tpcc_dh.n10.r1.log:     [java]            Stock Level:     54377 ( 40.5%)         0 (  0.0%)    906.28 txn/s   8202.70 ms
    hstore_tpcc_dh.n10.r1.log:     [java]                Payment:       169 (  0.1%)       169 (100.0%)      2.82 txn/s  52645.87 ms
    hstore_tpcc_dh.n10.r1.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n10.r1.log:     [java]           Order Status:     43256 ( 32.3%)         0 (  0.0%)    720.93 txn/s   8250.06 ms
    hstore_tpcc_dh.n1.r0.log:     [java] Throughput:     34238.87 txn/s [min:31675.20 / max:39538.40 / stdev:2865.42]
    hstore_tpcc_dh.n1.r0.log:     [java]               Delivery:     92033 (  4.5%)         0 (  0.0%)   1533.88 txn/s  10215.79 ms
    hstore_tpcc_dh.n1.r0.log:     [java]              New Order:    936091 ( 45.6%)       203 (  0.0%)  15601.52 txn/s  10760.32 ms
    hstore_tpcc_dh.n1.r0.log:     [java]            Stock Level:    114996 (  5.6%)         0 (  0.0%)   1916.60 txn/s   9962.03 ms
    hstore_tpcc_dh.n1.r0.log:     [java]                Payment:    841889 ( 41.0%)       244 (  0.0%)  14031.48 txn/s  10945.95 ms
    hstore_tpcc_dh.n1.r0.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n1.r0.log:     [java]           Order Status:     69323 (  3.4%)         0 (  0.0%)   1155.38 txn/s   9923.34 ms
    hstore_tpcc_dh.n1.r1.log:     [java] Throughput:     35656.67 txn/s [min:14246.20 / max:79520.10 / stdev:23946.28]
    hstore_tpcc_dh.n1.r1.log:     [java]               Delivery:     96485 (  4.5%)         0 (  0.0%)   1608.08 txn/s   9201.85 ms
    hstore_tpcc_dh.n1.r1.log:     [java]              New Order:    974434 ( 45.5%)       348 (  0.0%)  16240.57 txn/s   9896.51 ms
    hstore_tpcc_dh.n1.r1.log:     [java]            Stock Level:     97247 (  4.5%)         0 (  0.0%)   1620.78 txn/s   9006.40 ms
    hstore_tpcc_dh.n1.r1.log:     [java]                Payment:    898751 ( 42.0%)       279 (  0.0%)  14979.18 txn/s   9848.36 ms
    hstore_tpcc_dh.n1.r1.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n1.r1.log:     [java]           Order Status:     72483 (  3.4%)         0 (  0.0%)   1208.05 txn/s   8994.26 ms
    hstore_tpcc_dh.n2.r0.log:     [java] Throughput:     30223.80 txn/s [min:20378.20 / max:52798.80 / stdev:12905.62]
    hstore_tpcc_dh.n2.r0.log:     [java]               Delivery:     92945 (  5.1%)         0 (  0.0%)   1549.08 txn/s   9139.65 ms
    hstore_tpcc_dh.n2.r0.log:     [java]              New Order:    832675 ( 45.9%)       181 (  0.0%)  13877.92 txn/s   9573.89 ms
    hstore_tpcc_dh.n2.r0.log:     [java]            Stock Level:    116297 (  6.4%)         0 (  0.0%)   1938.28 txn/s   8973.45 ms
    hstore_tpcc_dh.n2.r0.log:     [java]                Payment:    678071 ( 37.4%)       190 (  0.0%)  11301.18 txn/s   9657.06 ms
    hstore_tpcc_dh.n2.r0.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n2.r0.log:     [java]           Order Status:     93440 (  5.2%)         0 (  0.0%)   1557.33 txn/s   8906.30 ms
    hstore_tpcc_dh.n3.r0.log:     [java] Throughput:     17954.57 txn/s [min:10048.80 / max:30124.00 / stdev:6935.33]
    hstore_tpcc_dh.n3.r0.log:     [java]               Delivery:     64131 (  6.0%)         0 (  0.0%)   1068.85 txn/s  11822.11 ms
    hstore_tpcc_dh.n3.r0.log:     [java]              New Order:    495036 ( 46.0%)       111 (  0.0%)   8250.60 txn/s  12242.53 ms
    hstore_tpcc_dh.n3.r0.log:     [java]            Stock Level:     64953 (  6.0%)         0 (  0.0%)   1082.55 txn/s  11690.87 ms
    hstore_tpcc_dh.n3.r0.log:     [java]                Payment:    388814 ( 36.1%)       144 (  0.0%)   6480.23 txn/s  12315.84 ms
    hstore_tpcc_dh.n3.r0.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n3.r0.log:     [java]           Order Status:     64340 (  6.0%)         0 (  0.0%)   1072.33 txn/s  11712.77 ms
    hstore_tpcc_dh.n3.r1.log:     [java] Throughput:     26296.22 txn/s [min:14154.90 / max:50332.50 / stdev:13631.07]
    hstore_tpcc_dh.n3.r1.log:     [java]               Delivery:     94187 (  6.0%)         0 (  0.0%)   1569.78 txn/s   8113.99 ms
    hstore_tpcc_dh.n3.r1.log:     [java]              New Order:    754877 ( 47.8%)       189 (  0.0%)  12581.28 txn/s   8667.62 ms
    hstore_tpcc_dh.n3.r1.log:     [java]            Stock Level:     94203 (  6.0%)         0 (  0.0%)   1570.05 txn/s   7836.45 ms
    hstore_tpcc_dh.n3.r1.log:     [java]                Payment:    540213 ( 34.2%)       234 (  0.0%)   9003.55 txn/s   8822.64 ms
    hstore_tpcc_dh.n3.r1.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n3.r1.log:     [java]           Order Status:     94293 (  6.0%)         0 (  0.0%)   1571.55 txn/s   7907.20 ms
    hstore_tpcc_dh.n5.r1.log:     [java] Throughput:     13139.72 txn/s [min:5833.90 / max:21191.80 / stdev:6023.19]
    hstore_tpcc_dh.n5.r1.log:     [java]               Delivery:     68905 (  8.7%)         0 (  0.0%)   1148.42 txn/s   9176.07 ms
    hstore_tpcc_dh.n5.r1.log:     [java]              New Order:    380158 ( 48.2%)       117 (  0.0%)   6335.97 txn/s   9519.18 ms
    hstore_tpcc_dh.n5.r1.log:     [java]            Stock Level:     85871 ( 10.9%)         0 (  0.0%)   1431.18 txn/s   9114.05 ms
    hstore_tpcc_dh.n5.r1.log:     [java]                Payment:    184958 ( 23.5%)        39 (  0.0%)   3082.63 txn/s   9519.93 ms
    hstore_tpcc_dh.n5.r1.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n5.r1.log:     [java]           Order Status:     68491 (  8.7%)         0 (  0.0%)   1141.52 txn/s   9073.16 ms
    hstore_tpcc_dh.n6.r0.log:     [java] Throughput:     6972.05 txn/s [min:4816.50 / max:10475.50 / stdev:2015.41]
    hstore_tpcc_dh.n6.r0.log:     [java]               Delivery:     49023 ( 11.7%)         0 (  0.0%)    817.05 txn/s   9679.18 ms
    hstore_tpcc_dh.n6.r0.log:     [java]              New Order:    218052 ( 52.1%)        78 (  0.0%)   3634.20 txn/s  10003.19 ms
    hstore_tpcc_dh.n6.r0.log:     [java]            Stock Level:     48774 ( 11.7%)         0 (  0.0%)    812.90 txn/s   9530.40 ms
    hstore_tpcc_dh.n6.r0.log:     [java]                Payment:     53639 ( 12.8%)        24 (  0.0%)    893.98 txn/s   9957.82 ms
    hstore_tpcc_dh.n6.r0.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n6.r0.log:     [java]           Order Status:     48835 ( 11.7%)         0 (  0.0%)    813.92 txn/s   9519.87 ms
    hstore_tpcc_dh.n9.r1.log:     [java] Throughput:     2615.38 txn/s [min:964.70 / max:4932.80 / stdev:1580.20]
    hstore_tpcc_dh.n9.r1.log:     [java]               Delivery:     46845 ( 29.9%)         0 (  0.0%)    780.75 txn/s   8059.33 ms
    hstore_tpcc_dh.n9.r1.log:     [java]              New Order:     44421 ( 28.3%)       239 (  0.5%)    740.35 txn/s   8389.87 ms
    hstore_tpcc_dh.n9.r1.log:     [java]            Stock Level:     28115 ( 17.9%)         0 (  0.0%)    468.58 txn/s   7823.71 ms
    hstore_tpcc_dh.n9.r1.log:     [java]                Payment:       195 (  0.1%)       195 (100.0%)      3.25 txn/s  53017.50 ms
    hstore_tpcc_dh.n9.r1.log:     [java]        Reset Warehouse:         0 (  0.0%)         0 (  0.0%)      0.00 txn/s         - ms
    hstore_tpcc_dh.n9.r1.log:     [java]           Order Status:     37347 ( 23.8%)         0 (  0.0%)    622.45 txn/s   7860.01 ms

This result is without HTT.
Still the crash issue happens 50%. Some of these results are partial for that reason.

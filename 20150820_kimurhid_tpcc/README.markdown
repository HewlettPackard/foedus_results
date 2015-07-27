
1. Perforamnce Regression test after https://github.com/hkimura/foedus_code/commit/f1899fe62602b25382ab0914d1bcef93e5c0a0a5.

Dragonhawk, in-memory, as usual.
20150719_tpcc_dh.tar.gz

    result_tpcc_dh.n0.r0.log: 11.1476
    result_tpcc_dh.n0.r1.log: 11.128
    result_tpcc_dh.n0.r2.log: 11.1447
    result_tpcc_dh.n1.r0.log: 10.5593
    result_tpcc_dh.n1.r1.log: 10.5584
    result_tpcc_dh.n1.r2.log: 10.4897
    result_tpcc_dh.n2.r0.log: 10.2685
    result_tpcc_dh.n3.r0.log: 10.1585
    result_tpcc_dh.n3.r1.log: 10.1219
    result_tpcc_dh.n3.r2.log: 10.1797
    result_tpcc_dh.n4.r0.log: 10.0653
    result_tpcc_dh.n4.r1.log: 10.0618
    result_tpcc_dh.n4.r2.log: 9.95107
    result_tpcc_dh.n5.r0.log: 9.8315
    result_tpcc_dh.n5.r1.log: 10.0282
    result_tpcc_dh.n5.r2.log: 9.92991
    result_tpcc_dh.n6.r0.log: 9.89762
    result_tpcc_dh.n6.r1.log: 9.88247
    result_tpcc_dh.n6.r2.log: 9.80337
    result_tpcc_dh.n7.r0.log: 9.80675
    result_tpcc_dh.n7.r1.log: 9.75261
    result_tpcc_dh.n7.r2.log: 9.81274
    result_tpcc_dh.n8.r0.log: 9.69422
    result_tpcc_dh.n8.r1.log: 10.2955
    result_tpcc_dh.n8.r2.log: 10.6296
    result_tpcc_dh.n9.r0.log: 10.7636
    result_tpcc_dh.n9.r1.log: 10.3395
    result_tpcc_dh.n9.r2.log: 9.96364
    result_tpcc_dh.n10.r0.log: 9.61707
    result_tpcc_dh.n10.r1.log: 9.60303
    result_tpcc_dh.n10.r2.log: 9.46494

Okay, seems good.


2. Another regression test after switching to glog-0.3.4

Same. 20150726_tpcc_dh_gcc.tar.gz

**GCC**

    result_tpcc_dh.n0.r0.log: 11.3419
    result_tpcc_dh.n0.r1.log: 11.3024
    result_tpcc_dh.n0.r2.log: 11.2356
    result_tpcc_dh.n1.r0.log: 10.8978
    result_tpcc_dh.n1.r1.log: 10.7639
    result_tpcc_dh.n1.r2.log: 10.9887
    result_tpcc_dh.n2.r0.log: 10.8537
    result_tpcc_dh.n2.r1.log: 10.9193
    result_tpcc_dh.n2.r2.log: 11.0141
    result_tpcc_dh.n3.r0.log: 10.8034
    result_tpcc_dh.n3.r1.log: 10.7134
    result_tpcc_dh.n3.r2.log: 10.7799
    result_tpcc_dh.n4.r0.log: 10.5771
    result_tpcc_dh.n4.r1.log: 10.6184
    result_tpcc_dh.n4.r2.log: 10.5646
    result_tpcc_dh.n5.r0.log: 10.5364
    result_tpcc_dh.n5.r1.log: 10.641
    result_tpcc_dh.n5.r2.log: 10.6136
    result_tpcc_dh.n6.r0.log: 10.1131
    result_tpcc_dh.n6.r1.log: 10.614
    result_tpcc_dh.n6.r2.log: 10.2199
    result_tpcc_dh.n7.r0.log: 9.97216
    result_tpcc_dh.n7.r1.log: 10.1933
    result_tpcc_dh.n7.r2.log: 10.17
    result_tpcc_dh.n8.r0.log: 10.3847
    result_tpcc_dh.n8.r1.log: 10.2818
    result_tpcc_dh.n8.r2.log: 10.3108
    result_tpcc_dh.n9.r0.log: 10.2203
    result_tpcc_dh.n9.r1.log: 10.4781
    result_tpcc_dh.n9.r2.log: 10.2459
    result_tpcc_dh.n10.r0.log: 10.1563
    result_tpcc_dh.n10.r1.log: 10.3107
    result_tpcc_dh.n10.r2.log: 10.3675

Again, okay. Actually slightly faster? (a few changes over the week)
I bet it's a fluke tho.



3. Yet another regression test using clang

Same. 20150726_tpcc_dh_clang.tar.gz

**CLANG** Hooray.
However, this time we used clang just as the front-end compiler.
I still linked to gcc's libstdc++ and also use /usr/bin/ld without switching the default
(didn't like to do intrusive thing in smaug). Also haven't tried "-flto". Got some issues with it.

Actually, even this basic setting didn't work so I had to compile on DL580 (where it works
although both of them are RHEL7.0!), then uploaded the binary to smaug.
Same issue as this guy: http://stackoverflow.com/questions/26380407/cmake-clang-is-not-able-compile-a-simple-test-program-fedora-20

Anyways..


    result_tpcc_dh.n0.r0.log: 11.3676
    result_tpcc_dh.n0.r1.log: 11.5368
    result_tpcc_dh.n0.r2.log: 11.4099
    result_tpcc_dh.n1.r0.log: 11.0887
    result_tpcc_dh.n1.r1.log: 10.9743
    result_tpcc_dh.n1.r2.log: 11.1948
    result_tpcc_dh.n2.r0.log: 10.8377
    result_tpcc_dh.n2.r1.log: 10.8051
    result_tpcc_dh.n2.r2.log: 10.7547
    result_tpcc_dh.n3.r0.log: 10.6803
    result_tpcc_dh.n3.r1.log: 10.6203
    result_tpcc_dh.n3.r2.log: 10.9018
    result_tpcc_dh.n4.r0.log: 10.685
    result_tpcc_dh.n4.r1.log: 10.5629
    result_tpcc_dh.n4.r2.log: 10.6311
    result_tpcc_dh.n5.r0.log: 10.4514
    result_tpcc_dh.n5.r1.log: 10.6839
    result_tpcc_dh.n5.r2.log: 10.6792
    result_tpcc_dh.n6.r0.log: 10.2679
    result_tpcc_dh.n6.r1.log: 10.3846
    result_tpcc_dh.n6.r2.log: 10.2346
    result_tpcc_dh.n7.r0.log: 10.3453
    result_tpcc_dh.n7.r1.log: 10.398
    result_tpcc_dh.n7.r2.log: 10.5479
    result_tpcc_dh.n8.r0.log: 10.272
    result_tpcc_dh.n8.r1.log: 10.2809
    result_tpcc_dh.n8.r2.log: 10.4145
    result_tpcc_dh.n9.r0.log: 10.2806
    result_tpcc_dh.n9.r1.log: 10.3711
    result_tpcc_dh.n9.r2.log: 10.1689
    result_tpcc_dh.n10.r0.log: 10.2785
    result_tpcc_dh.n10.r1.log: 10.2456
    result_tpcc_dh.n10.r2.log: 10.2814

Basically same. Expected.

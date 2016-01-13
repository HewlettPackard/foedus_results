HCC YCSB results
========
Abrv.
* "dh" means smaug, "gh" means puff.
* "ro" means read-only workload (add-read=10). "rw" means read-write.

Results
* 20160105_hcc_ycsb_dh.tar.gz : Used run_ycsb_f_dh.sh
* 20160107_hcc_ycsb_dh_incomplete.tar.gz: Varied threshold, but it was incomplete because one experiment didn't finish.
* 20160109_hcc_ycsb_dh_ro.tar.gz : threshold 0 and 50. read-only.
* 20160109_hcc_ycsb_dl580_ro_prof : same as above, except on DL580. CPU profile.
* 20160109_hcc_ycsb_dh_rw.tar.gz : read-write. threshold 0, 50, 100, 256. size 1000, 10000, addres 0, 2, 4, 6, 8, 10.
* 20160111_hcc_ycsb_dh_rw2.tar.gz : read-write. same as above, but new code.
* 20160109_hcc_ycsb_dl580_ro.tar.gz : Used the ro script.
* 20160109_hcc_ycsb_z820_ro.tar.gz : Used the ro script.
* 20160111_hcc_ycsb_hp840_ro.tar : Read-only YCSB-F on HP840 laptop; running and result generation scripts included.
* 20160113_hcc_ycsb_gh_ro.tar.gz: Used the ro script.

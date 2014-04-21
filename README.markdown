Empirical result files for libfoedus
=================================

What this is
-----------
This repository contains all experimental results and other binary files that should be
better separated from source code.

House rule: Upload your experimental results to keep track of them
-----------
It's also very often that other people or yourself lose track of where experimental results
are, which version of the program they were based on, etc.

Upload all experimental results, raw and processed, to the foedus_results git repository.
The repository is separated from the main foedus_code repo to keep it compact.
Again, do *NOT* upload the results to main foedus_code repo.

Each experimental result should be placed in its own folder, ideally tar-ed into one file.
You should also contain glog files (e.g /tmp/libfoedus.INFO), not just std out.

See 20140414_kimurhid_array_readonly for example.

Folder naming rule
-----------
YYYYMMDD_yourname_title
eg: 20140414_kimurhid_array_readonly


What each folder contains
-----------
It should at least contain README.markdown.
README.markdown should describe at least the followings:

* Your name (contact)
* Experiment (give full path of the experiment)
* When you ran it: Date
* Version of the source code
* Experimental Environemnt
* Configurations etc
* Details: Anything notable.


Here is an example.
```text
Contact: kimurhid
Experiment: foedus/storage/array/readonly_experiment.cpp
Date: 2014/04/21


Version
-------
Master latest as of 2014/04/21 noon.

Environment
-------
My Z820. 16 cores, 128GB memory. Release build.

Details
-------
300-320 MQPS for 16-bytes payload.
One note is that I observed a significantly different throughput by placing
"foedus::memory::AlignedMemory numbers_" as a member variable or a local variable.
If it's member variable, I get 300MQPS. If local variable (although I call release_block()
anyways), 150MQPS. It shouldn't affect anything. Mistery.
```

If there are any scripts or files that would help re-running the experiments, put it there.
Results files are ideally tar-ed into one file, but not mandatory.

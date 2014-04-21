Contact: kimurhid
Experiment: foedus/storage/array/readonly_experiment.cpp
Date: 2014/04/21

Version
-------
Master latest as of 2014/04/21 noon.

Environment
-------
Z820. 16 cores, 128GB memory. Release build.

Details
-------
300-320 MQPS for 16-bytes payload. 70 MQPS for 128-bytes payload (memcpy bottleneck).
One note is that I observed a significantly different throughput by placing
"foedus::memory::AlignedMemory numbers_" as a member variable or a local variable.
If it's member variable, I get 300MQPS. If local variable (although I call release_block()
anyways), 150MQPS. It shouldn't affect anything. Mistery.



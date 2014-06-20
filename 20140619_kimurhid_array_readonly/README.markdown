Contact: kimurhid
Experiment: foedus/storage/array/readonly_experiment.cpp
Date: 2014/06/19

Version
-------
Master latest as of 2014/06/19 noon.

Environment
-------
Z820. 16 cores, 128GB memory. Release build.

Details
-------
400 MQPS for 16-bytes payload. 100 MQPS for 128-bytes payload (memcpy bottleneck).
Quite a lot improved from 04/14 exclusing memcpy bottleneck.

Improvments:

* Optimized integer division in array lookup.
* Light versions of get_record that return ErrorCode, not ErrorStack.
* A few other minor things.

Results (16b payload)
--------
all started!
I'm done! 256, processed=254017536
I'm done! 262, processed=255066112
I'm done! 1, processed=249626624
I'm done! 257, processed=254148608
I'm done! 260, processed=238616576
I'm done! I'm done! 261, processed=251920384
2, processed=240975872
I'm done! 0, processed=250871808
I'm done! 258, processed=254672896
I'm done! 4, processed=251789312
session: result[I'm done! I'm done! 263, processed=7255918080
, processed=250871808
0]=No error
I'm done! 6, processed=245563392
I'm done! 259, processed=254738432
I'm done! I'm done! 53, processed=250806272
, processed=250019840
session: result[1]=No error
session: result[2]=No error
session: result[3]=No error
session: result[4]=No error
session: result[5]=No error
session: result[6]=No error
session: result[7]=No error
session: result[8]=No error
session: result[9]=No error
session: result[10]=No error
session: result[11]=No error
session: result[12]=No error
session: result[13]=No error
session: result[14]=No error
session: result[15]=No error
total=4009115142, MQPS=400.912



Results (128b payload)
--------
all started!
I'm done! 260, processed=62980096
I'm done! 257, processed=64290816
I'm done! I'm done! 40, processed=, processed=6291456062849024

session: result[0]=No error
I'm done! 5, processed=62717952
I'm done! 263, processed=62586880I'm done! 
3, processed=63111168
I'm done! 262, processed=64159744
I'm done! 7, processed=63176704
I'm done! 2, processed=62062592
I'm done! I'm done! 256, processed=64421888
6, processed=61145088
I'm done! 259, processed=64028672
I'm done! 258, processed=64356352
I'm done! 261, processed=64159744
I'm done! 1, processed=62849024
session: result[1]=No error
session: result[2]=No error
session: result[3]=No error
session: result[4]=No error
session: result[5]=No error
session: result[6]=No error
session: result[7]=No error
session: result[8]=No error
session: result[9]=No error
session: result[10]=No error
session: result[11]=No error
session: result[12]=No error
session: result[13]=No error
session: result[14]=No error
session: result[15]=No error

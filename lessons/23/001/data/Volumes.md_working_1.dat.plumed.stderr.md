Stderr for source:  Volumes.md_working_1.dat   
Download: [zipped raw stdout](Volumes.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Volumes.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action INSPHERE with label sp : keyword DATA is compulsory for this action
[fv-az1106-805:41141] *** Process received signal ***
[fv-az1106-805:41141] Signal: Aborted (6)
[fv-az1106-805:41141] Signal code:  (-6)
[fv-az1106-805:41141] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f76f0442520]
[fv-az1106-805:41141] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f76f04969fc]
[fv-az1106-805:41141] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f76f0442476]
[fv-az1106-805:41141] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f76f04287f3]
[fv-az1106-805:41141] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f76f08a2b9e]
[fv-az1106-805:41141] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f76f08ae20c]
[fv-az1106-805:41141] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f76f08ae277]
[fv-az1106-805:41141] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f76f08ae52b]
[fv-az1106-805:41141] [ 8] plumed(+0x12f48)[0x555943a74f48]
[fv-az1106-805:41141] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f76f0429d90]
[fv-az1106-805:41141] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f76f0429e40]
[fv-az1106-805:41141] [11] plumed(+0x131e5)[0x555943a751e5]
[fv-az1106-805:41141] *** End of error message ***
</pre>
{% endraw %}

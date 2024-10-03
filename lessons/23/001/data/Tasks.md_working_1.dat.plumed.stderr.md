Stderr for source:  Tasks.md_working_1.dat   
Download: [zipped raw stdout](Tasks.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-650:41952] *** Process received signal ***
[fv-az714-650:41952] Signal: Aborted (6)
[fv-az714-650:41952] Signal code:  (-6)
[fv-az714-650:41952] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1bc2642520]
[fv-az714-650:41952] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1bc26969fc]
[fv-az714-650:41952] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1bc2642476]
[fv-az714-650:41952] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1bc26287f3]
[fv-az714-650:41952] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1bc2aa2b9e]
[fv-az714-650:41952] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1bc2aae20c]
[fv-az714-650:41952] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1bc2aae277]
[fv-az714-650:41952] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1bc2aae52b]
[fv-az714-650:41952] [ 8] plumed(+0x12f48)[0x55dcdc3d5f48]
[fv-az714-650:41952] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1bc2629d90]
[fv-az714-650:41952] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1bc2629e40]
[fv-az714-650:41952] [11] plumed(+0x131e5)[0x55dcdc3d61e5]
[fv-az714-650:41952] *** End of error message ***
</pre>
{% endraw %}

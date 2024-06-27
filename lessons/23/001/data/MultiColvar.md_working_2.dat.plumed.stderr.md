Stderr for source:  MultiColvar.md_working_2.dat   
Download: [zipped raw stdout](MultiColvar.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvar.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:39556] *** Process received signal ***
[fv-az1106-805:39556] Signal: Aborted (6)
[fv-az1106-805:39556] Signal code:  (-6)
[fv-az1106-805:39556] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff8e4042520]
[fv-az1106-805:39556] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff8e40969fc]
[fv-az1106-805:39556] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff8e4042476]
[fv-az1106-805:39556] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff8e40287f3]
[fv-az1106-805:39556] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff8e44a2b9e]
[fv-az1106-805:39556] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff8e44ae20c]
[fv-az1106-805:39556] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff8e44ae277]
[fv-az1106-805:39556] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff8e44ae52b]
[fv-az1106-805:39556] [ 8] plumed(+0x12f48)[0x555ba5c3ef48]
[fv-az1106-805:39556] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff8e4029d90]
[fv-az1106-805:39556] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff8e4029e40]
[fv-az1106-805:39556] [11] plumed(+0x131e5)[0x555ba5c3f1e5]
[fv-az1106-805:39556] *** End of error message ***
</pre>
{% endraw %}

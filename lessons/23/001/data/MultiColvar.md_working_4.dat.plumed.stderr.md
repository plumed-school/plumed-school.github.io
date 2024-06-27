Stderr for source:  MultiColvar.md_working_4.dat   
Download: [zipped raw stdout](MultiColvar.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvar.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:39647] *** Process received signal ***
[fv-az1106-805:39647] Signal: Aborted (6)
[fv-az1106-805:39647] Signal code:  (-6)
[fv-az1106-805:39647] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f444a442520]
[fv-az1106-805:39647] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f444a4969fc]
[fv-az1106-805:39647] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f444a442476]
[fv-az1106-805:39647] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f444a4287f3]
[fv-az1106-805:39647] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f444a8a2b9e]
[fv-az1106-805:39647] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f444a8ae20c]
[fv-az1106-805:39647] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f444a8ae277]
[fv-az1106-805:39647] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f444a8ae52b]
[fv-az1106-805:39647] [ 8] plumed(+0x12f48)[0x5588c58a4f48]
[fv-az1106-805:39647] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f444a429d90]
[fv-az1106-805:39647] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f444a429e40]
[fv-az1106-805:39647] [11] plumed(+0x131e5)[0x5588c58a51e5]
[fv-az1106-805:39647] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  MultiColvar.md_working_3.dat   
Download: [zipped raw stdout](MultiColvar.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvar.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:39603] *** Process received signal ***
[fv-az1106-805:39603] Signal: Aborted (6)
[fv-az1106-805:39603] Signal code:  (-6)
[fv-az1106-805:39603] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9188842520]
[fv-az1106-805:39603] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f91888969fc]
[fv-az1106-805:39603] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9188842476]
[fv-az1106-805:39603] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f91888287f3]
[fv-az1106-805:39603] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f9188ca2b9e]
[fv-az1106-805:39603] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f9188cae20c]
[fv-az1106-805:39603] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f9188cae277]
[fv-az1106-805:39603] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9188cae52b]
[fv-az1106-805:39603] [ 8] plumed(+0x12f48)[0x564a0934df48]
[fv-az1106-805:39603] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9188829d90]
[fv-az1106-805:39603] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9188829e40]
[fv-az1106-805:39603] [11] plumed(+0x131e5)[0x564a0934e1e5]
[fv-az1106-805:39603] *** End of error message ***
</pre>
{% endraw %}

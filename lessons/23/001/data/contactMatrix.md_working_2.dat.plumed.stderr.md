Stderr for source:  contactMatrix.md_working_2.dat   
Download: [zipped raw stdout](contactMatrix.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az1106-805:39861] *** Process received signal ***
[fv-az1106-805:39861] Signal: Aborted (6)
[fv-az1106-805:39861] Signal code:  (-6)
[fv-az1106-805:39861] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb171642520]
[fv-az1106-805:39861] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb1716969fc]
[fv-az1106-805:39861] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb171642476]
[fv-az1106-805:39861] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb1716287f3]
[fv-az1106-805:39861] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb171aa2b9e]
[fv-az1106-805:39861] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb171aae20c]
[fv-az1106-805:39861] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb171aae277]
[fv-az1106-805:39861] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb171aae52b]
[fv-az1106-805:39861] [ 8] plumed(+0x12f48)[0x55e5afe70f48]
[fv-az1106-805:39861] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb171629d90]
[fv-az1106-805:39861] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb171629e40]
[fv-az1106-805:39861] [11] plumed(+0x131e5)[0x55e5afe711e5]
[fv-az1106-805:39861] *** End of error message ***
</pre>
{% endraw %}

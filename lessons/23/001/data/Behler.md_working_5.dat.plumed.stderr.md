Stderr for source:  Behler.md_working_5.dat   
Download: [zipped raw stdout](Behler.md_working_5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Behler.md_working_5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az1106-805:41079] *** Process received signal ***
[fv-az1106-805:41079] Signal: Aborted (6)
[fv-az1106-805:41079] Signal code:  (-6)
[fv-az1106-805:41079] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2395442520]
[fv-az1106-805:41079] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f23954969fc]
[fv-az1106-805:41079] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2395442476]
[fv-az1106-805:41079] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f23954287f3]
[fv-az1106-805:41079] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f23958a2b9e]
[fv-az1106-805:41079] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f23958ae20c]
[fv-az1106-805:41079] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f23958ae277]
[fv-az1106-805:41079] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f23958ae52b]
[fv-az1106-805:41079] [ 8] plumed(+0x12f48)[0x55824cb46f48]
[fv-az1106-805:41079] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2395429d90]
[fv-az1106-805:41079] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2395429e40]
[fv-az1106-805:41079] [11] plumed(+0x131e5)[0x55824cb471e5]
[fv-az1106-805:41079] *** End of error message ***
</pre>
{% endraw %}

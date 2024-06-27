Stderr for source:  Behler.md_working_4.dat   
Download: [zipped raw stdout](Behler.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Behler.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:41048] *** Process received signal ***
[fv-az1106-805:41048] Signal: Aborted (6)
[fv-az1106-805:41048] Signal code:  (-6)
[fv-az1106-805:41048] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6df7842520]
[fv-az1106-805:41048] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6df78969fc]
[fv-az1106-805:41048] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6df7842476]
[fv-az1106-805:41048] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6df78287f3]
[fv-az1106-805:41048] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6df7ca2b9e]
[fv-az1106-805:41048] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6df7cae20c]
[fv-az1106-805:41048] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6df7cae277]
[fv-az1106-805:41048] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6df7cae52b]
[fv-az1106-805:41048] [ 8] plumed(+0x12f48)[0x55b0c9667f48]
[fv-az1106-805:41048] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6df7829d90]
[fv-az1106-805:41048] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6df7829e40]
[fv-az1106-805:41048] [11] plumed(+0x131e5)[0x55b0c96681e5]
[fv-az1106-805:41048] *** End of error message ***
</pre>
{% endraw %}

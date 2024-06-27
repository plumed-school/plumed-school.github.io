Stderr for source:  Tasks.md_working_2.dat   
Download: [zipped raw stdout](Tasks.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:40157] *** Process received signal ***
[fv-az1106-805:40157] Signal: Aborted (6)
[fv-az1106-805:40157] Signal code:  (-6)
[fv-az1106-805:40157] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5100842520]
[fv-az1106-805:40157] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f51008969fc]
[fv-az1106-805:40157] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5100842476]
[fv-az1106-805:40157] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f51008287f3]
[fv-az1106-805:40157] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5100ca2b9e]
[fv-az1106-805:40157] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5100cae20c]
[fv-az1106-805:40157] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5100cae277]
[fv-az1106-805:40157] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5100cae52b]
[fv-az1106-805:40157] [ 8] plumed(+0x12f48)[0x55b79b11ef48]
[fv-az1106-805:40157] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5100829d90]
[fv-az1106-805:40157] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5100829e40]
[fv-az1106-805:40157] [11] plumed(+0x131e5)[0x55b79b11f1e5]
[fv-az1106-805:40157] *** End of error message ***
</pre>
{% endraw %}

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
[fv-az1106-805:40113] *** Process received signal ***
[fv-az1106-805:40113] Signal: Aborted (6)
[fv-az1106-805:40113] Signal code:  (-6)
[fv-az1106-805:40113] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6fe6a42520]
[fv-az1106-805:40113] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6fe6a969fc]
[fv-az1106-805:40113] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6fe6a42476]
[fv-az1106-805:40113] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6fe6a287f3]
[fv-az1106-805:40113] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6fe6ea2b9e]
[fv-az1106-805:40113] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6fe6eae20c]
[fv-az1106-805:40113] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6fe6eae277]
[fv-az1106-805:40113] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6fe6eae52b]
[fv-az1106-805:40113] [ 8] plumed(+0x12f48)[0x55afed062f48]
[fv-az1106-805:40113] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6fe6a29d90]
[fv-az1106-805:40113] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6fe6a29e40]
[fv-az1106-805:40113] [11] plumed(+0x131e5)[0x55afed0631e5]
[fv-az1106-805:40113] *** End of error message ***
</pre>
{% endraw %}

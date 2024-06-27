Stderr for source:  MultiColvarShortcut.md_working_2.dat   
Download: [zipped raw stdout](MultiColvarShortcut.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvarShortcut.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az1106-805:39710] *** Process received signal ***
[fv-az1106-805:39710] Signal: Aborted (6)
[fv-az1106-805:39710] Signal code:  (-6)
[fv-az1106-805:39710] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe641042520]
[fv-az1106-805:39710] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe6410969fc]
[fv-az1106-805:39710] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe641042476]
[fv-az1106-805:39710] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe6410287f3]
[fv-az1106-805:39710] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe6414a2b9e]
[fv-az1106-805:39710] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe6414ae20c]
[fv-az1106-805:39710] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe6414ae277]
[fv-az1106-805:39710] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe6414ae52b]
[fv-az1106-805:39710] [ 8] plumed(+0x12f48)[0x561444507f48]
[fv-az1106-805:39710] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe641029d90]
[fv-az1106-805:39710] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe641029e40]
[fv-az1106-805:39710] [11] plumed(+0x131e5)[0x5614445081e5]
[fv-az1106-805:39710] *** End of error message ***
</pre>
{% endraw %}

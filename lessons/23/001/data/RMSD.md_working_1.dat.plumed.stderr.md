Stderr for source:  RMSD.md_working_1.dat   
Download: [zipped raw stdout](RMSD.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONSTANT with label v : cannot understand the following words from the input line : NCOLS=12, NROWS=2
[fv-az1106-805:42262] *** Process received signal ***
[fv-az1106-805:42262] Signal: Aborted (6)
[fv-az1106-805:42262] Signal code:  (-6)
[fv-az1106-805:42262] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3b8b242520]
[fv-az1106-805:42262] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3b8b2969fc]
[fv-az1106-805:42262] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3b8b242476]
[fv-az1106-805:42262] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3b8b2287f3]
[fv-az1106-805:42262] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3b8b6a2b9e]
[fv-az1106-805:42262] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3b8b6ae20c]
[fv-az1106-805:42262] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3b8b6ae277]
[fv-az1106-805:42262] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3b8b6ae52b]
[fv-az1106-805:42262] [ 8] plumed(+0x12f48)[0x5610272ddf48]
[fv-az1106-805:42262] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3b8b229d90]
[fv-az1106-805:42262] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3b8b229e40]
[fv-az1106-805:42262] [11] plumed(+0x131e5)[0x5610272de1e5]
[fv-az1106-805:42262] *** End of error message ***
</pre>
{% endraw %}

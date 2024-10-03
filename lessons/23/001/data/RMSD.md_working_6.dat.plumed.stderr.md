Stderr for source:  RMSD.md_working_6.dat   
Download: [zipped raw stdout](RMSD.md_working_6.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_6.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action RMSD with label rmsd : cannot understand the following words from the input line : DISPLACEMENT
[fv-az714-650:44252] *** Process received signal ***
[fv-az714-650:44252] Signal: Aborted (6)
[fv-az714-650:44252] Signal code:  (-6)
[fv-az714-650:44252] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4ca3042520]
[fv-az714-650:44252] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4ca30969fc]
[fv-az714-650:44252] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4ca3042476]
[fv-az714-650:44252] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4ca30287f3]
[fv-az714-650:44252] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4ca34a2b9e]
[fv-az714-650:44252] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4ca34ae20c]
[fv-az714-650:44252] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4ca34ae277]
[fv-az714-650:44252] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4ca34ae52b]
[fv-az714-650:44252] [ 8] plumed(+0x12f48)[0x55e19bf15f48]
[fv-az714-650:44252] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4ca3029d90]
[fv-az714-650:44252] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4ca3029e40]
[fv-az714-650:44252] [11] plumed(+0x131e5)[0x55e19bf161e5]
[fv-az714-650:44252] *** End of error message ***
</pre>
{% endraw %}

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
[fv-az1106-805:42411] *** Process received signal ***
[fv-az1106-805:42411] Signal: Aborted (6)
[fv-az1106-805:42411] Signal code:  (-6)
[fv-az1106-805:42411] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f706b842520]
[fv-az1106-805:42411] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f706b8969fc]
[fv-az1106-805:42411] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f706b842476]
[fv-az1106-805:42411] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f706b8287f3]
[fv-az1106-805:42411] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f706bca2b9e]
[fv-az1106-805:42411] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f706bcae20c]
[fv-az1106-805:42411] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f706bcae277]
[fv-az1106-805:42411] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f706bcae52b]
[fv-az1106-805:42411] [ 8] plumed(+0x12f48)[0x5595d0a4bf48]
[fv-az1106-805:42411] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f706b829d90]
[fv-az1106-805:42411] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f706b829e40]
[fv-az1106-805:42411] [11] plumed(+0x131e5)[0x5595d0a4c1e5]
[fv-az1106-805:42411] *** End of error message ***
</pre>
{% endraw %}

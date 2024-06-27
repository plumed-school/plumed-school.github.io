Stderr for source:  Sprint.md_working_1.dat   
Download: [zipped raw stdout](Sprint.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Sprint.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action SPRINT with label s1 : keyword MATRIX is compulsory for this action
[fv-az1106-805:40284] *** Process received signal ***
[fv-az1106-805:40284] Signal: Aborted (6)
[fv-az1106-805:40284] Signal code:  (-6)
[fv-az1106-805:40284] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd1a3642520]
[fv-az1106-805:40284] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd1a36969fc]
[fv-az1106-805:40284] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd1a3642476]
[fv-az1106-805:40284] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd1a36287f3]
[fv-az1106-805:40284] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd1a3aa2b9e]
[fv-az1106-805:40284] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd1a3aae20c]
[fv-az1106-805:40284] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd1a3aae277]
[fv-az1106-805:40284] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd1a3aae52b]
[fv-az1106-805:40284] [ 8] plumed(+0x12f48)[0x55624119ff48]
[fv-az1106-805:40284] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd1a3629d90]
[fv-az1106-805:40284] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd1a3629e40]
[fv-az1106-805:40284] [11] plumed(+0x131e5)[0x5562411a01e5]
[fv-az1106-805:40284] *** End of error message ***
</pre>
{% endraw %}

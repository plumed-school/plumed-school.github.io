Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : keyword SIGMA could not be read correctly
[fv-az1106-805:42600] *** Process received signal ***
[fv-az1106-805:42600] Signal: Aborted (6)
[fv-az1106-805:42600] Signal code:  (-6)
[fv-az1106-805:42600] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fadc0c42520]
[fv-az1106-805:42600] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fadc0c969fc]
[fv-az1106-805:42600] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fadc0c42476]
[fv-az1106-805:42600] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fadc0c287f3]
[fv-az1106-805:42600] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fadc10a2b9e]
[fv-az1106-805:42600] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fadc10ae20c]
[fv-az1106-805:42600] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fadc10ae277]
[fv-az1106-805:42600] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fadc10ae52b]
[fv-az1106-805:42600] [ 8] plumed_master(+0x14274)[0x55a512d92274]
[fv-az1106-805:42600] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fadc0c29d90]
[fv-az1106-805:42600] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fadc0c29e40]
[fv-az1106-805:42600] [11] plumed_master(+0x14ed5)[0x55a512d92ed5]
[fv-az1106-805:42600] *** End of error message ***
</pre>
{% endraw %}

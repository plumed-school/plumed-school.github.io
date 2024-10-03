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
[fv-az740-873:42073] *** Process received signal ***
[fv-az740-873:42073] Signal: Aborted (6)
[fv-az740-873:42073] Signal code:  (-6)
[fv-az740-873:42073] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f22eea42520]
[fv-az740-873:42073] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f22eea969fc]
[fv-az740-873:42073] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f22eea42476]
[fv-az740-873:42073] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f22eea287f3]
[fv-az740-873:42073] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f22eeea2b9e]
[fv-az740-873:42073] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f22eeeae20c]
[fv-az740-873:42073] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f22eeeae277]
[fv-az740-873:42073] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f22eeeae52b]
[fv-az740-873:42073] [ 8] plumed_master(+0x14274)[0x55b3261e4274]
[fv-az740-873:42073] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f22eea29d90]
[fv-az740-873:42073] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f22eea29e40]
[fv-az740-873:42073] [11] plumed_master(+0x14ed5)[0x55b3261e4ed5]
[fv-az740-873:42073] *** End of error message ***
</pre>
{% endraw %}

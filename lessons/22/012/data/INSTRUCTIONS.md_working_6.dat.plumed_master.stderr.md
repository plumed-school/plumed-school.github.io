Stderr for source:  INSTRUCTIONS.md_working_6.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_6.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_6.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action UPPER_WALLS with label @s9 : cannot find action named cv (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[fv-az740-873:42195] *** Process received signal ***
[fv-az740-873:42195] Signal: Aborted (6)
[fv-az740-873:42195] Signal code:  (-6)
[fv-az740-873:42195] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8ef8442520]
[fv-az740-873:42195] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8ef84969fc]
[fv-az740-873:42195] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8ef8442476]
[fv-az740-873:42195] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8ef84287f3]
[fv-az740-873:42195] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8ef88a2b9e]
[fv-az740-873:42195] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8ef88ae20c]
[fv-az740-873:42195] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8ef88ae277]
[fv-az740-873:42195] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8ef88ae52b]
[fv-az740-873:42195] [ 8] plumed_master(+0x14274)[0x55d021e45274]
[fv-az740-873:42195] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8ef8429d90]
[fv-az740-873:42195] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8ef8429e40]
[fv-az740-873:42195] [11] plumed_master(+0x14ed5)[0x55d021e45ed5]
[fv-az740-873:42195] *** End of error message ***
</pre>
{% endraw %}

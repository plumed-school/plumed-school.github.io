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
[fv-az1106-805:42722] *** Process received signal ***
[fv-az1106-805:42722] Signal: Aborted (6)
[fv-az1106-805:42722] Signal code:  (-6)
[fv-az1106-805:42722] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8078442520]
[fv-az1106-805:42722] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f80784969fc]
[fv-az1106-805:42722] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8078442476]
[fv-az1106-805:42722] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f80784287f3]
[fv-az1106-805:42722] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f80788a2b9e]
[fv-az1106-805:42722] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f80788ae20c]
[fv-az1106-805:42722] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f80788ae277]
[fv-az1106-805:42722] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f80788ae52b]
[fv-az1106-805:42722] [ 8] plumed_master(+0x14274)[0x562c09c6d274]
[fv-az1106-805:42722] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8078429d90]
[fv-az1106-805:42722] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8078429e40]
[fv-az1106-805:42722] [11] plumed_master(+0x14ed5)[0x562c09c6ded5]
[fv-az1106-805:42722] *** End of error message ***
</pre>
{% endraw %}

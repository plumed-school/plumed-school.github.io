Stderr for source:  INSTRUCTIONS.md_working_7.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_7.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_7.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[fv-az714-382:08793] *** Process received signal ***
[fv-az714-382:08793] Signal: Aborted (6)
[fv-az714-382:08793] Signal code:  (-6)
[fv-az714-382:08793] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4c2c042520]
[fv-az714-382:08793] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4c2c0969fc]
[fv-az714-382:08793] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4c2c042476]
[fv-az714-382:08793] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4c2c0287f3]
[fv-az714-382:08793] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4c2c4a2b9e]
[fv-az714-382:08793] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4c2c4ae20c]
[fv-az714-382:08793] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4c2c4ae277]
[fv-az714-382:08793] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4c2c4ae52b]
[fv-az714-382:08793] [ 8] plumed_master(+0x14274)[0x564ce4d37274]
[fv-az714-382:08793] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4c2c029d90]
[fv-az714-382:08793] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4c2c029e40]
[fv-az714-382:08793] [11] plumed_master(+0x14ed5)[0x564ce4d37ed5]
[fv-az714-382:08793] *** End of error message ***
</pre>
{% endraw %}

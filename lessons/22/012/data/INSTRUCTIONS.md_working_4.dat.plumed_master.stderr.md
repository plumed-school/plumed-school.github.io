Stderr for source:  INSTRUCTIONS.md_working_4.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[fv-az1106-805:42660] *** Process received signal ***
[fv-az1106-805:42660] Signal: Aborted (6)
[fv-az1106-805:42660] Signal code:  (-6)
[fv-az1106-805:42660] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1546842520]
[fv-az1106-805:42660] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f15468969fc]
[fv-az1106-805:42660] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1546842476]
[fv-az1106-805:42660] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f15468287f3]
[fv-az1106-805:42660] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1546ca2b9e]
[fv-az1106-805:42660] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1546cae20c]
[fv-az1106-805:42660] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1546cae277]
[fv-az1106-805:42660] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1546cae52b]
[fv-az1106-805:42660] [ 8] plumed_master(+0x14274)[0x5651ac854274]
[fv-az1106-805:42660] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1546829d90]
[fv-az1106-805:42660] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1546829e40]
[fv-az1106-805:42660] [11] plumed_master(+0x14ed5)[0x5651ac854ed5]
[fv-az1106-805:42660] *** End of error message ***
</pre>
{% endraw %}

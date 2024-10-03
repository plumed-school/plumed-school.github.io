Stderr for source:  INSTRUCTIONS.md_working_10.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_10.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_10.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label dist : could not find file named colvar_reweight.data
[fv-az1205-759:41666] *** Process received signal ***
[fv-az1205-759:41666] Signal: Aborted (6)
[fv-az1205-759:41666] Signal code:  (-6)
[fv-az1205-759:41666] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa335842520]
[fv-az1205-759:41666] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa3358969fc]
[fv-az1205-759:41666] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa335842476]
[fv-az1205-759:41666] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa3358287f3]
[fv-az1205-759:41666] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa335ca2b9e]
[fv-az1205-759:41666] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa335cae20c]
[fv-az1205-759:41666] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa335cae277]
[fv-az1205-759:41666] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa335cae52b]
[fv-az1205-759:41666] [ 8] plumed_master(+0x14274)[0x562f516f7274]
[fv-az1205-759:41666] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa335829d90]
[fv-az1205-759:41666] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa335829e40]
[fv-az1205-759:41666] [11] plumed_master(+0x14ed5)[0x562f516f7ed5]
[fv-az1205-759:41666] *** End of error message ***
</pre>
{% endraw %}

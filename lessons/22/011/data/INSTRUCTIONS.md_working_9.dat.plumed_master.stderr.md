Stderr for source:  INSTRUCTIONS.md_working_9.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_9.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_9.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action READ with label dist : could not find file named colvar_reweight.data
[fv-az1205-759:41634] *** Process received signal ***
[fv-az1205-759:41634] Signal: Aborted (6)
[fv-az1205-759:41634] Signal code:  (-6)
[fv-az1205-759:41634] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f311b442520]
[fv-az1205-759:41634] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f311b4969fc]
[fv-az1205-759:41634] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f311b442476]
[fv-az1205-759:41634] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f311b4287f3]
[fv-az1205-759:41634] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f311b8a2b9e]
[fv-az1205-759:41634] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f311b8ae20c]
[fv-az1205-759:41634] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f311b8ae277]
[fv-az1205-759:41634] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f311b8ae52b]
[fv-az1205-759:41634] [ 8] plumed_master(+0x14274)[0x560cbeb25274]
[fv-az1205-759:41634] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f311b429d90]
[fv-az1205-759:41634] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f311b429e40]
[fv-az1205-759:41634] [11] plumed_master(+0x14ed5)[0x560cbeb25ed5]
[fv-az1205-759:41634] *** End of error message ***
</pre>
{% endraw %}

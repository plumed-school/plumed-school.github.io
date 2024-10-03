Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DFSCLUSTERING with label dfs : keyword ARG is compulsory for this action
[fv-az1205-759:41889] *** Process received signal ***
[fv-az1205-759:41889] Signal: Aborted (6)
[fv-az1205-759:41889] Signal code:  (-6)
[fv-az1205-759:41889] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f130be42520]
[fv-az1205-759:41889] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f130be969fc]
[fv-az1205-759:41889] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f130be42476]
[fv-az1205-759:41889] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f130be287f3]
[fv-az1205-759:41889] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f130c2a2b9e]
[fv-az1205-759:41889] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f130c2ae20c]
[fv-az1205-759:41889] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f130c2ae277]
[fv-az1205-759:41889] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f130c2ae52b]
[fv-az1205-759:41889] [ 8] plumed_master(+0x14274)[0x55b8e8218274]
[fv-az1205-759:41889] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f130be29d90]
[fv-az1205-759:41889] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f130be29e40]
[fv-az1205-759:41889] [11] plumed_master(+0x14ed5)[0x55b8e8218ed5]
[fv-az1205-759:41889] *** End of error message ***
</pre>
{% endraw %}

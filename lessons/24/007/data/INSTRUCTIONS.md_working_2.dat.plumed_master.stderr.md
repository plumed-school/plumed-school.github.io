Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[fv-az740-873:41327] *** Process received signal ***
[fv-az740-873:41327] Signal: Aborted (6)
[fv-az740-873:41327] Signal code:  (-6)
[fv-az740-873:41327] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe05e642520]
[fv-az740-873:41327] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe05e6969fc]
[fv-az740-873:41327] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe05e642476]
[fv-az740-873:41327] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe05e6287f3]
[fv-az740-873:41327] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe05eaa2b9e]
[fv-az740-873:41327] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe05eaae20c]
[fv-az740-873:41327] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe05eaae277]
[fv-az740-873:41327] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe05eaae52b]
[fv-az740-873:41327] [ 8] plumed_master(+0x14274)[0x563453234274]
[fv-az740-873:41327] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe05e629d90]
[fv-az740-873:41327] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe05e629e40]
[fv-az740-873:41327] [11] plumed_master(+0x14ed5)[0x563453234ed5]
[fv-az740-873:41327] *** End of error message ***
</pre>
{% endraw %}

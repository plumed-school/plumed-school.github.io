Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action MORE_THAN_VECTOR with label nclust_mt : problem reading SWITCH keyword : could not parse D_0
[fv-az714-382:08888] *** Process received signal ***
[fv-az714-382:08888] Signal: Aborted (6)
[fv-az714-382:08888] Signal code:  (-6)
[fv-az714-382:08888] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6ab1e42520]
[fv-az714-382:08888] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6ab1e969fc]
[fv-az714-382:08888] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6ab1e42476]
[fv-az714-382:08888] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6ab1e287f3]
[fv-az714-382:08888] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6ab22a2b9e]
[fv-az714-382:08888] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6ab22ae20c]
[fv-az714-382:08888] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6ab22ae277]
[fv-az714-382:08888] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6ab22ae52b]
[fv-az714-382:08888] [ 8] plumed_master(+0x14274)[0x5593f9815274]
[fv-az714-382:08888] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6ab1e29d90]
[fv-az714-382:08888] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6ab1e29e40]
[fv-az714-382:08888] [11] plumed_master(+0x14ed5)[0x5593f9815ed5]
[fv-az714-382:08888] *** End of error message ***
</pre>
{% endraw %}

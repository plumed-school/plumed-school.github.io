Stderr for source:  manual/data/specifying_arguments.md_working_4.dat   
Download: [zipped raw stdout](specifying_arguments.md_working_4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](specifying_arguments.md_working_4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action PRINT with label @2 : found no element in d3 with label y.d3.z
[fv-az740-873:40668] *** Process received signal ***
[fv-az740-873:40668] Signal: Aborted (6)
[fv-az740-873:40668] Signal code:  (-6)
[fv-az740-873:40668] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f84c9c42520]
[fv-az740-873:40668] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f84c9c969fc]
[fv-az740-873:40668] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f84c9c42476]
[fv-az740-873:40668] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f84c9c287f3]
[fv-az740-873:40668] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f84ca0a2b9e]
[fv-az740-873:40668] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f84ca0ae20c]
[fv-az740-873:40668] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f84ca0ae277]
[fv-az740-873:40668] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f84ca0ae52b]
[fv-az740-873:40668] [ 8] plumed_master(+0x14274)[0x55db6d8c6274]
[fv-az740-873:40668] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f84c9c29d90]
[fv-az740-873:40668] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f84c9c29e40]
[fv-az740-873:40668] [11] plumed_master(+0x14ed5)[0x55db6d8c6ed5]
[fv-az740-873:40668] *** End of error message ***
</pre>
{% endraw %}

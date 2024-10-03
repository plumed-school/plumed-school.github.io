Stderr for source:  postprocessing.md_working_5.dat   
Download: [zipped raw stdout](postprocessing.md_working_5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](postprocessing.md_working_5.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @18 : keyword ARG is compulsory for this action
[fv-az740-873:41910] *** Process received signal ***
[fv-az740-873:41910] Signal: Aborted (6)
[fv-az740-873:41910] Signal code:  (-6)
[fv-az740-873:41910] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8a9e642520]
[fv-az740-873:41910] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8a9e6969fc]
[fv-az740-873:41910] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8a9e642476]
[fv-az740-873:41910] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8a9e6287f3]
[fv-az740-873:41910] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8a9eaa2b9e]
[fv-az740-873:41910] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8a9eaae20c]
[fv-az740-873:41910] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8a9eaae277]
[fv-az740-873:41910] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8a9eaae52b]
[fv-az740-873:41910] [ 8] plumed_master(+0x14274)[0x5584d2e7d274]
[fv-az740-873:41910] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8a9e629d90]
[fv-az740-873:41910] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8a9e629e40]
[fv-az740-873:41910] [11] plumed_master(+0x14ed5)[0x5584d2e7ded5]
[fv-az740-873:41910] *** End of error message ***
</pre>
{% endraw %}

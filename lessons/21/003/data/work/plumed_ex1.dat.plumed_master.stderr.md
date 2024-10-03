Stderr for source:  work/plumed_ex1.dat   
Download: [zipped raw stdout](plumed_ex1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @35 : keyword ARG is compulsory for this action
[fv-az740-873:42529] *** Process received signal ***
[fv-az740-873:42529] Signal: Aborted (6)
[fv-az740-873:42529] Signal code:  (-6)
[fv-az740-873:42529] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc9ca442520]
[fv-az740-873:42529] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc9ca4969fc]
[fv-az740-873:42529] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc9ca442476]
[fv-az740-873:42529] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc9ca4287f3]
[fv-az740-873:42529] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc9ca8a2b9e]
[fv-az740-873:42529] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc9ca8ae20c]
[fv-az740-873:42529] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc9ca8ae277]
[fv-az740-873:42529] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc9ca8ae52b]
[fv-az740-873:42529] [ 8] plumed_master(+0x14274)[0x55997403c274]
[fv-az740-873:42529] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc9ca429d90]
[fv-az740-873:42529] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc9ca429e40]
[fv-az740-873:42529] [11] plumed_master(+0x14ed5)[0x55997403ced5]
[fv-az740-873:42529] *** End of error message ***
</pre>
{% endraw %}

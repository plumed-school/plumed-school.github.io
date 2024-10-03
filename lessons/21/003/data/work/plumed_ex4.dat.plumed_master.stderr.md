Stderr for source:  work/plumed_ex4.dat   
Download: [zipped raw stdout](plumed_ex4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @33 : keyword ARG is compulsory for this action
[fv-az740-873:42618] *** Process received signal ***
[fv-az740-873:42618] Signal: Aborted (6)
[fv-az740-873:42618] Signal code:  (-6)
[fv-az740-873:42618] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2419e42520]
[fv-az740-873:42618] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2419e969fc]
[fv-az740-873:42618] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2419e42476]
[fv-az740-873:42618] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2419e287f3]
[fv-az740-873:42618] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f241a2a2b9e]
[fv-az740-873:42618] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f241a2ae20c]
[fv-az740-873:42618] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f241a2ae277]
[fv-az740-873:42618] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f241a2ae52b]
[fv-az740-873:42618] [ 8] plumed_master(+0x14274)[0x559779a49274]
[fv-az740-873:42618] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2419e29d90]
[fv-az740-873:42618] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2419e29e40]
[fv-az740-873:42618] [11] plumed_master(+0x14ed5)[0x559779a49ed5]
[fv-az740-873:42618] *** End of error message ***
</pre>
{% endraw %}

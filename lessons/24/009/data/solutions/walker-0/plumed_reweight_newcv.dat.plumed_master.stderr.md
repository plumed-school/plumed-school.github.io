Stderr for source:  ./solutions/walker-0/plumed_reweight_newcv.dat   
Download: [zipped raw stdout](plumed_reweight_newcv.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_newcv.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @33 : keyword ARG is compulsory for this action
[fv-az740-873:41263] *** Process received signal ***
[fv-az740-873:41263] Signal: Aborted (6)
[fv-az740-873:41263] Signal code:  (-6)
[fv-az740-873:41263] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa34e842520]
[fv-az740-873:41263] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa34e8969fc]
[fv-az740-873:41263] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa34e842476]
[fv-az740-873:41263] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa34e8287f3]
[fv-az740-873:41263] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa34eca2b9e]
[fv-az740-873:41263] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa34ecae20c]
[fv-az740-873:41263] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa34ecae277]
[fv-az740-873:41263] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa34ecae52b]
[fv-az740-873:41263] [ 8] plumed_master(+0x14274)[0x55eaec6f3274]
[fv-az740-873:41263] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa34e829d90]
[fv-az740-873:41263] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa34e829e40]
[fv-az740-873:41263] [11] plumed_master(+0x14ed5)[0x55eaec6f3ed5]
[fv-az740-873:41263] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex2.dat   
Download: [zipped raw stdout](plumed_ex2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @38 : keyword ARG is compulsory for this action
[fv-az740-873:42559] *** Process received signal ***
[fv-az740-873:42559] Signal: Aborted (6)
[fv-az740-873:42559] Signal code:  (-6)
[fv-az740-873:42559] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe98d242520]
[fv-az740-873:42559] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe98d2969fc]
[fv-az740-873:42559] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe98d242476]
[fv-az740-873:42559] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe98d2287f3]
[fv-az740-873:42559] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe98d6a2b9e]
[fv-az740-873:42559] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe98d6ae20c]
[fv-az740-873:42559] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe98d6ae277]
[fv-az740-873:42559] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe98d6ae52b]
[fv-az740-873:42559] [ 8] plumed_master(+0x14274)[0x55a286c44274]
[fv-az740-873:42559] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe98d229d90]
[fv-az740-873:42559] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe98d229e40]
[fv-az740-873:42559] [11] plumed_master(+0x14ed5)[0x55a286c44ed5]
[fv-az740-873:42559] *** End of error message ***
</pre>
{% endraw %}

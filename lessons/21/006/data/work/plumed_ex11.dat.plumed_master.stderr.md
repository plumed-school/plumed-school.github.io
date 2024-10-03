Stderr for source:  work/plumed_ex11.dat   
Download: [zipped raw stdout](plumed_ex11.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex11.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @63 : keyword ARG is compulsory for this action
[fv-az659-187:42304] *** Process received signal ***
[fv-az659-187:42304] Signal: Aborted (6)
[fv-az659-187:42304] Signal code:  (-6)
[fv-az659-187:42304] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa79c842520]
[fv-az659-187:42304] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa79c8969fc]
[fv-az659-187:42304] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa79c842476]
[fv-az659-187:42304] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa79c8287f3]
[fv-az659-187:42304] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa79cca2b9e]
[fv-az659-187:42304] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa79ccae20c]
[fv-az659-187:42304] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa79ccae277]
[fv-az659-187:42304] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa79ccae52b]
[fv-az659-187:42304] [ 8] plumed_master(+0x14274)[0x55ccb447b274]
[fv-az659-187:42304] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa79c829d90]
[fv-az659-187:42304] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa79c829e40]
[fv-az659-187:42304] [11] plumed_master(+0x14ed5)[0x55ccb447bed5]
[fv-az659-187:42304] *** End of error message ***
</pre>
{% endraw %}

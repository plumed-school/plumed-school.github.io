Stderr for source:  MultiColvar.md_working_2.dat   
Download: [zipped raw stdout](MultiColvar.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvar.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-650:41393] *** Process received signal ***
[fv-az714-650:41393] Signal: Aborted (6)
[fv-az714-650:41393] Signal code:  (-6)
[fv-az714-650:41393] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fed0fe42520]
[fv-az714-650:41393] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fed0fe969fc]
[fv-az714-650:41393] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fed0fe42476]
[fv-az714-650:41393] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fed0fe287f3]
[fv-az714-650:41393] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fed102a2b9e]
[fv-az714-650:41393] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fed102ae20c]
[fv-az714-650:41393] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fed102ae277]
[fv-az714-650:41393] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fed102ae52b]
[fv-az714-650:41393] [ 8] plumed(+0x12f48)[0x5637aec7df48]
[fv-az714-650:41393] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fed0fe29d90]
[fv-az714-650:41393] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fed0fe29e40]
[fv-az714-650:41393] [11] plumed(+0x131e5)[0x5637aec7e1e5]
[fv-az714-650:41393] *** End of error message ***
</pre>
{% endraw %}

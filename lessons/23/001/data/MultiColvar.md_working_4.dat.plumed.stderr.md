Stderr for source:  MultiColvar.md_working_4.dat   
Download: [zipped raw stdout](MultiColvar.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MultiColvar.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-382:05650] *** Process received signal ***
[fv-az714-382:05650] Signal: Aborted (6)
[fv-az714-382:05650] Signal code:  (-6)
[fv-az714-382:05650] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd0efa42520]
[fv-az714-382:05650] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd0efa969fc]
[fv-az714-382:05650] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd0efa42476]
[fv-az714-382:05650] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd0efa287f3]
[fv-az714-382:05650] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd0efea2b9e]
[fv-az714-382:05650] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd0efeae20c]
[fv-az714-382:05650] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd0efeae277]
[fv-az714-382:05650] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd0efeae52b]
[fv-az714-382:05650] [ 8] plumed(+0x12f48)[0x5596b1d7ef48]
[fv-az714-382:05650] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd0efa29d90]
[fv-az714-382:05650] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd0efa29e40]
[fv-az714-382:05650] [11] plumed(+0x131e5)[0x5596b1d7f1e5]
[fv-az714-382:05650] *** End of error message ***
</pre>
{% endraw %}

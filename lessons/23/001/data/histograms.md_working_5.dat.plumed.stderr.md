Stderr for source:  histograms.md_working_5.dat   
Download: [zipped raw stdout](histograms.md_working_5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-650:43723] *** Process received signal ***
[fv-az714-650:43723] Signal: Aborted (6)
[fv-az714-650:43723] Signal code:  (-6)
[fv-az714-650:43723] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f491a042520]
[fv-az714-650:43723] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f491a0969fc]
[fv-az714-650:43723] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f491a042476]
[fv-az714-650:43723] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f491a0287f3]
[fv-az714-650:43723] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f491a4a2b9e]
[fv-az714-650:43723] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f491a4ae20c]
[fv-az714-650:43723] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f491a4ae277]
[fv-az714-650:43723] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f491a4ae52b]
[fv-az714-650:43723] [ 8] plumed(+0x12f48)[0x55656585af48]
[fv-az714-650:43723] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f491a029d90]
[fv-az714-650:43723] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f491a029e40]
[fv-az714-650:43723] [11] plumed(+0x131e5)[0x55656585b1e5]
[fv-az714-650:43723] *** End of error message ***
</pre>
{% endraw %}

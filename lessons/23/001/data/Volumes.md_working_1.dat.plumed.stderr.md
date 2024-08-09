Stderr for source:  Volumes.md_working_1.dat   
Download: [zipped raw stdout](Volumes.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Volumes.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action INSPHERE with label sp : keyword DATA is compulsory for this action
[fv-az714-382:07166] *** Process received signal ***
[fv-az714-382:07166] Signal: Aborted (6)
[fv-az714-382:07166] Signal code:  (-6)
[fv-az714-382:07166] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f21bda42520]
[fv-az714-382:07166] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f21bda969fc]
[fv-az714-382:07166] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f21bda42476]
[fv-az714-382:07166] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f21bda287f3]
[fv-az714-382:07166] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f21bdea2b9e]
[fv-az714-382:07166] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f21bdeae20c]
[fv-az714-382:07166] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f21bdeae277]
[fv-az714-382:07166] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f21bdeae52b]
[fv-az714-382:07166] [ 8] plumed(+0x12f48)[0x557acb82df48]
[fv-az714-382:07166] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f21bda29d90]
[fv-az714-382:07166] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f21bda29e40]
[fv-az714-382:07166] [11] plumed(+0x131e5)[0x557acb82e1e5]
[fv-az714-382:07166] *** End of error message ***
</pre>
{% endraw %}

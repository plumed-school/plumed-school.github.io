Stderr for source:  Tasks.md_working_1.dat   
Download: [zipped raw stdout](Tasks.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-382:06122] *** Process received signal ***
[fv-az714-382:06122] Signal: Aborted (6)
[fv-az714-382:06122] Signal code:  (-6)
[fv-az714-382:06122] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f113c642520]
[fv-az714-382:06122] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f113c6969fc]
[fv-az714-382:06122] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f113c642476]
[fv-az714-382:06122] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f113c6287f3]
[fv-az714-382:06122] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f113caa2b9e]
[fv-az714-382:06122] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f113caae20c]
[fv-az714-382:06122] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f113caae277]
[fv-az714-382:06122] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f113caae52b]
[fv-az714-382:06122] [ 8] plumed(+0x12f48)[0x562e9a5bdf48]
[fv-az714-382:06122] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f113c629d90]
[fv-az714-382:06122] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f113c629e40]
[fv-az714-382:06122] [11] plumed(+0x131e5)[0x562e9a5be1e5]
[fv-az714-382:06122] *** End of error message ***
</pre>
{% endraw %}

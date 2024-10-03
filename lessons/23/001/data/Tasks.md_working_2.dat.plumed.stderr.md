Stderr for source:  Tasks.md_working_2.dat   
Download: [zipped raw stdout](Tasks.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-650:41996] *** Process received signal ***
[fv-az714-650:41996] Signal: Aborted (6)
[fv-az714-650:41996] Signal code:  (-6)
[fv-az714-650:41996] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f858d042520]
[fv-az714-650:41996] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f858d0969fc]
[fv-az714-650:41996] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f858d042476]
[fv-az714-650:41996] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f858d0287f3]
[fv-az714-650:41996] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f858d4a2b9e]
[fv-az714-650:41996] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f858d4ae20c]
[fv-az714-650:41996] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f858d4ae277]
[fv-az714-650:41996] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f858d4ae52b]
[fv-az714-650:41996] [ 8] plumed(+0x12f48)[0x564a76683f48]
[fv-az714-650:41996] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f858d029d90]
[fv-az714-650:41996] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f858d029e40]
[fv-az714-650:41996] [11] plumed(+0x131e5)[0x564a766841e5]
[fv-az714-650:41996] *** End of error message ***
</pre>
{% endraw %}

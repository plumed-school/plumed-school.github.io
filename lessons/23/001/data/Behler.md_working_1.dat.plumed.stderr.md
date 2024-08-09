Stderr for source:  Behler.md_working_1.dat   
Download: [zipped raw stdout](Behler.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Behler.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az714-382:06984] *** Process received signal ***
[fv-az714-382:06984] Signal: Aborted (6)
[fv-az714-382:06984] Signal code:  (-6)
[fv-az714-382:06984] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7faedf642520]
[fv-az714-382:06984] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7faedf6969fc]
[fv-az714-382:06984] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7faedf642476]
[fv-az714-382:06984] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7faedf6287f3]
[fv-az714-382:06984] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7faedfaa2b9e]
[fv-az714-382:06984] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7faedfaae20c]
[fv-az714-382:06984] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7faedfaae277]
[fv-az714-382:06984] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7faedfaae52b]
[fv-az714-382:06984] [ 8] plumed(+0x12f48)[0x55e557639f48]
[fv-az714-382:06984] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7faedf629d90]
[fv-az714-382:06984] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7faedf629e40]
[fv-az714-382:06984] [11] plumed(+0x131e5)[0x55e55763a1e5]
[fv-az714-382:06984] *** End of error message ***
</pre>
{% endraw %}

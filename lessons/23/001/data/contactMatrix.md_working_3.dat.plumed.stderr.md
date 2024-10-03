Stderr for source:  contactMatrix.md_working_3.dat   
Download: [zipped raw stdout](contactMatrix.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-650:41741] *** Process received signal ***
[fv-az714-650:41741] Signal: Aborted (6)
[fv-az714-650:41741] Signal code:  (-6)
[fv-az714-650:41741] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9154242520]
[fv-az714-650:41741] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f91542969fc]
[fv-az714-650:41741] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9154242476]
[fv-az714-650:41741] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f91542287f3]
[fv-az714-650:41741] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f91546a2b9e]
[fv-az714-650:41741] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f91546ae20c]
[fv-az714-650:41741] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f91546ae277]
[fv-az714-650:41741] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f91546ae52b]
[fv-az714-650:41741] [ 8] plumed(+0x12f48)[0x5641ee167f48]
[fv-az714-650:41741] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9154229d90]
[fv-az714-650:41741] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9154229e40]
[fv-az714-650:41741] [11] plumed(+0x131e5)[0x5641ee1681e5]
[fv-az714-650:41741] *** End of error message ***
</pre>
{% endraw %}

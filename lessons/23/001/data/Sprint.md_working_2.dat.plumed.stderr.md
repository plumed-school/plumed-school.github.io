Stderr for source:  Sprint.md_working_2.dat   
Download: [zipped raw stdout](Sprint.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Sprint.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label s1_mat : No atoms have been read in
[fv-az714-650:42151] *** Process received signal ***
[fv-az714-650:42151] Signal: Aborted (6)
[fv-az714-650:42151] Signal code:  (-6)
[fv-az714-650:42151] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6539442520]
[fv-az714-650:42151] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f65394969fc]
[fv-az714-650:42151] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6539442476]
[fv-az714-650:42151] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f65394287f3]
[fv-az714-650:42151] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f65398a2b9e]
[fv-az714-650:42151] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f65398ae20c]
[fv-az714-650:42151] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f65398ae277]
[fv-az714-650:42151] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f65398ae52b]
[fv-az714-650:42151] [ 8] plumed(+0x12f48)[0x55e095bb5f48]
[fv-az714-650:42151] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6539429d90]
[fv-az714-650:42151] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6539429e40]
[fv-az714-650:42151] [11] plumed(+0x131e5)[0x55e095bb61e5]
[fv-az714-650:42151] *** End of error message ***
</pre>
{% endraw %}

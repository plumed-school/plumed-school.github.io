Stderr for source:  Steinhardt.md_working_11.dat   
Download: [zipped raw stdout](Steinhardt.md_working_11.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_11.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az1106-805:40680] *** Process received signal ***
[fv-az1106-805:40680] Signal: Aborted (6)
[fv-az1106-805:40680] Signal code:  (-6)
[fv-az1106-805:40680] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8071e42520]
[fv-az1106-805:40680] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8071e969fc]
[fv-az1106-805:40680] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8071e42476]
[fv-az1106-805:40680] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8071e287f3]
[fv-az1106-805:40680] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f80722a2b9e]
[fv-az1106-805:40680] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f80722ae20c]
[fv-az1106-805:40680] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f80722ae277]
[fv-az1106-805:40680] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f80722ae52b]
[fv-az1106-805:40680] [ 8] plumed(+0x12f48)[0x5595b82f2f48]
[fv-az1106-805:40680] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8071e29d90]
[fv-az1106-805:40680] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8071e29e40]
[fv-az1106-805:40680] [11] plumed(+0x131e5)[0x5595b82f31e5]
[fv-az1106-805:40680] *** End of error message ***
</pre>
{% endraw %}

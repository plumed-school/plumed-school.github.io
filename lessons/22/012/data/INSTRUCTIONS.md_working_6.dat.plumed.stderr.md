Stderr for source:  INSTRUCTIONS.md_working_6.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_6.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_6.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action UPPER_WALLS with label uwall : cannot find action named cv (hint! the actions with value in this ActionSet are: )
[fv-az1106-805:42714] *** Process received signal ***
[fv-az1106-805:42714] Signal: Aborted (6)
[fv-az1106-805:42714] Signal code:  (-6)
[fv-az1106-805:42714] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f58f2642520]
[fv-az1106-805:42714] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f58f26969fc]
[fv-az1106-805:42714] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f58f2642476]
[fv-az1106-805:42714] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f58f26287f3]
[fv-az1106-805:42714] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f58f2aa2b9e]
[fv-az1106-805:42714] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f58f2aae20c]
[fv-az1106-805:42714] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f58f2aae277]
[fv-az1106-805:42714] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f58f2aae52b]
[fv-az1106-805:42714] [ 8] plumed(+0x12f48)[0x55d37117cf48]
[fv-az1106-805:42714] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f58f2629d90]
[fv-az1106-805:42714] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f58f2629e40]
[fv-az1106-805:42714] [11] plumed(+0x131e5)[0x55d37117d1e5]
[fv-az1106-805:42714] *** End of error message ***
</pre>
{% endraw %}

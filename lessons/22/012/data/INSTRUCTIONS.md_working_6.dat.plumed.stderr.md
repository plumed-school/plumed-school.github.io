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
[fv-az740-873:42187] *** Process received signal ***
[fv-az740-873:42187] Signal: Aborted (6)
[fv-az740-873:42187] Signal code:  (-6)
[fv-az740-873:42187] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd411e42520]
[fv-az740-873:42187] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd411e969fc]
[fv-az740-873:42187] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd411e42476]
[fv-az740-873:42187] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd411e287f3]
[fv-az740-873:42187] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd4122a2b9e]
[fv-az740-873:42187] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd4122ae20c]
[fv-az740-873:42187] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd4122ae277]
[fv-az740-873:42187] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd4122ae52b]
[fv-az740-873:42187] [ 8] plumed(+0x12f48)[0x558b74d5cf48]
[fv-az740-873:42187] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd411e29d90]
[fv-az740-873:42187] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd411e29e40]
[fv-az740-873:42187] [11] plumed(+0x131e5)[0x558b74d5d1e5]
[fv-az740-873:42187] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  INSTRUCTIONS.md_working_4.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: )
[fv-az740-873:42125] *** Process received signal ***
[fv-az740-873:42125] Signal: Aborted (6)
[fv-az740-873:42125] Signal code:  (-6)
[fv-az740-873:42125] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb5e6842520]
[fv-az740-873:42125] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb5e68969fc]
[fv-az740-873:42125] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb5e6842476]
[fv-az740-873:42125] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb5e68287f3]
[fv-az740-873:42125] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb5e6ca2b9e]
[fv-az740-873:42125] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb5e6cae20c]
[fv-az740-873:42125] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb5e6cae277]
[fv-az740-873:42125] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb5e6cae52b]
[fv-az740-873:42125] [ 8] plumed(+0x12f48)[0x55597e1a0f48]
[fv-az740-873:42125] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb5e6829d90]
[fv-az740-873:42125] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb5e6829e40]
[fv-az740-873:42125] [11] plumed(+0x131e5)[0x55597e1a11e5]
[fv-az740-873:42125] *** End of error message ***
</pre>
{% endraw %}

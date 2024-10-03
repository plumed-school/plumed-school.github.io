Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[fv-az740-873:41319] *** Process received signal ***
[fv-az740-873:41319] Signal: Aborted (6)
[fv-az740-873:41319] Signal code:  (-6)
[fv-az740-873:41319] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f12f8e42520]
[fv-az740-873:41319] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f12f8e969fc]
[fv-az740-873:41319] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f12f8e42476]
[fv-az740-873:41319] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f12f8e287f3]
[fv-az740-873:41319] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f12f92a2b9e]
[fv-az740-873:41319] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f12f92ae20c]
[fv-az740-873:41319] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f12f92ae277]
[fv-az740-873:41319] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f12f92ae52b]
[fv-az740-873:41319] [ 8] plumed(+0x12f48)[0x5637ff3c1f48]
[fv-az740-873:41319] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f12f8e29d90]
[fv-az740-873:41319] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f12f8e29e40]
[fv-az740-873:41319] [11] plumed(+0x131e5)[0x5637ff3c21e5]
[fv-az740-873:41319] *** End of error message ***
</pre>
{% endraw %}

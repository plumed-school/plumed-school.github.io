Stderr for source:  Steinhardt.md_working_10.dat   
Download: [zipped raw stdout](Steinhardt.md_working_10.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_10.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action PRINT with label @2 : action lq6 has no component named lq6 (hint! the components in this actions are: )
[fv-az714-382:06674] *** Process received signal ***
[fv-az714-382:06674] Signal: Aborted (6)
[fv-az714-382:06674] Signal code:  (-6)
[fv-az714-382:06674] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3403842520]
[fv-az714-382:06674] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f34038969fc]
[fv-az714-382:06674] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3403842476]
[fv-az714-382:06674] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f34038287f3]
[fv-az714-382:06674] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3403ca2b9e]
[fv-az714-382:06674] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3403cae20c]
[fv-az714-382:06674] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3403cae277]
[fv-az714-382:06674] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3403cae52b]
[fv-az714-382:06674] [ 8] plumed(+0x12f48)[0x55c16a36bf48]
[fv-az714-382:06674] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3403829d90]
[fv-az714-382:06674] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3403829e40]
[fv-az714-382:06674] [11] plumed(+0x131e5)[0x55c16a36c1e5]
[fv-az714-382:06674] *** End of error message ***
</pre>
{% endraw %}

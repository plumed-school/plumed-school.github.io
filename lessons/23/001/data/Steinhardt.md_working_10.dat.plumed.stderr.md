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
[fv-az714-650:42489] *** Process received signal ***
[fv-az714-650:42489] Signal: Aborted (6)
[fv-az714-650:42489] Signal code:  (-6)
[fv-az714-650:42489] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fee21442520]
[fv-az714-650:42489] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fee214969fc]
[fv-az714-650:42489] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fee21442476]
[fv-az714-650:42489] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fee214287f3]
[fv-az714-650:42489] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fee218a2b9e]
[fv-az714-650:42489] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fee218ae20c]
[fv-az714-650:42489] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fee218ae277]
[fv-az714-650:42489] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fee218ae52b]
[fv-az714-650:42489] [ 8] plumed(+0x12f48)[0x55f51e41ef48]
[fv-az714-650:42489] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fee21429d90]
[fv-az714-650:42489] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fee21429e40]
[fv-az714-650:42489] [11] plumed(+0x131e5)[0x55f51e41f1e5]
[fv-az714-650:42489] *** End of error message ***
</pre>
{% endraw %}

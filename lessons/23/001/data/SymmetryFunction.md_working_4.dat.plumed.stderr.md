Stderr for source:  SymmetryFunction.md_working_4.dat   
Download: [zipped raw stdout](SymmetryFunction.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](SymmetryFunction.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-650:43218] *** Process received signal ***
[fv-az714-650:43218] Signal: Aborted (6)
[fv-az714-650:43218] Signal code:  (-6)
[fv-az714-650:43218] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f79ad242520]
[fv-az714-650:43218] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f79ad2969fc]
[fv-az714-650:43218] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f79ad242476]
[fv-az714-650:43218] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f79ad2287f3]
[fv-az714-650:43218] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f79ad6a2b9e]
[fv-az714-650:43218] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f79ad6ae20c]
[fv-az714-650:43218] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f79ad6ae277]
[fv-az714-650:43218] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f79ad6ae52b]
[fv-az714-650:43218] [ 8] plumed(+0x12f48)[0x556276659f48]
[fv-az714-650:43218] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f79ad229d90]
[fv-az714-650:43218] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f79ad229e40]
[fv-az714-650:43218] [11] plumed(+0x131e5)[0x55627665a1e5]
[fv-az714-650:43218] *** End of error message ***
</pre>
{% endraw %}

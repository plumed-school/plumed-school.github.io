Stderr for source:  SymmetryFunction.md_working_5.dat   
Download: [zipped raw stdout](SymmetryFunction.md_working_5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](SymmetryFunction.md_working_5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-382:07456] *** Process received signal ***
[fv-az714-382:07456] Signal: Aborted (6)
[fv-az714-382:07456] Signal code:  (-6)
[fv-az714-382:07456] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4db7042520]
[fv-az714-382:07456] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4db70969fc]
[fv-az714-382:07456] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4db7042476]
[fv-az714-382:07456] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4db70287f3]
[fv-az714-382:07456] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4db74a2b9e]
[fv-az714-382:07456] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4db74ae20c]
[fv-az714-382:07456] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4db74ae277]
[fv-az714-382:07456] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4db74ae52b]
[fv-az714-382:07456] [ 8] plumed(+0x12f48)[0x5641e808df48]
[fv-az714-382:07456] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4db7029d90]
[fv-az714-382:07456] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4db7029e40]
[fv-az714-382:07456] [11] plumed(+0x131e5)[0x5641e808e1e5]
[fv-az714-382:07456] *** End of error message ***
</pre>
{% endraw %}

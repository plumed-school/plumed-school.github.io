Stderr for source:  Path.md_working_3.dat   
Download: [zipped raw stdout](Path.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Path.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GPATH LABEL=pp ARG=t1,t2 REFERENCE=epath.pdb
Maybe a missing space or a typo?
[fv-az714-382:08571] *** Process received signal ***
[fv-az714-382:08571] Signal: Aborted (6)
[fv-az714-382:08571] Signal code:  (-6)
[fv-az714-382:08571] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f74a0e42520]
[fv-az714-382:08571] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f74a0e969fc]
[fv-az714-382:08571] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f74a0e42476]
[fv-az714-382:08571] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f74a0e287f3]
[fv-az714-382:08571] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f74a12a2b9e]
[fv-az714-382:08571] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f74a12ae20c]
[fv-az714-382:08571] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f74a12ae277]
[fv-az714-382:08571] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f74a12ae52b]
[fv-az714-382:08571] [ 8] plumed(+0x12f48)[0x55e13a8eef48]
[fv-az714-382:08571] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f74a0e29d90]
[fv-az714-382:08571] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f74a0e29e40]
[fv-az714-382:08571] [11] plumed(+0x131e5)[0x55e13a8ef1e5]
[fv-az714-382:08571] *** End of error message ***
</pre>
{% endraw %}

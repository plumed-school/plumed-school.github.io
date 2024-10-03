Stderr for source:  contactMatrix.md_working_7.dat   
Download: [zipped raw stdout](contactMatrix.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ONES LABEL=ones64 SIZE=64
Maybe a missing space or a typo?
[fv-az714-650:41922] *** Process received signal ***
[fv-az714-650:41922] Signal: Aborted (6)
[fv-az714-650:41922] Signal code:  (-6)
[fv-az714-650:41922] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f622fc42520]
[fv-az714-650:41922] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f622fc969fc]
[fv-az714-650:41922] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f622fc42476]
[fv-az714-650:41922] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f622fc287f3]
[fv-az714-650:41922] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f62300a2b9e]
[fv-az714-650:41922] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f62300ae20c]
[fv-az714-650:41922] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f62300ae277]
[fv-az714-650:41922] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f62300ae52b]
[fv-az714-650:41922] [ 8] plumed(+0x12f48)[0x55bd08faef48]
[fv-az714-650:41922] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f622fc29d90]
[fv-az714-650:41922] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f622fc29e40]
[fv-az714-650:41922] [11] plumed(+0x131e5)[0x55bd08faf1e5]
[fv-az714-650:41922] *** End of error message ***
</pre>
{% endraw %}

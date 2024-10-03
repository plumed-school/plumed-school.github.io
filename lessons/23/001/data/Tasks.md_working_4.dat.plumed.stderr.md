Stderr for source:  Tasks.md_working_4.dat   
Download: [zipped raw stdout](Tasks.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ONES LABEL=ones SIZE=100
Maybe a missing space or a typo?
[fv-az714-650:42086] *** Process received signal ***
[fv-az714-650:42086] Signal: Aborted (6)
[fv-az714-650:42086] Signal code:  (-6)
[fv-az714-650:42086] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2c9ec42520]
[fv-az714-650:42086] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2c9ec969fc]
[fv-az714-650:42086] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2c9ec42476]
[fv-az714-650:42086] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2c9ec287f3]
[fv-az714-650:42086] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f2c9f0a2b9e]
[fv-az714-650:42086] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f2c9f0ae20c]
[fv-az714-650:42086] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f2c9f0ae277]
[fv-az714-650:42086] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f2c9f0ae52b]
[fv-az714-650:42086] [ 8] plumed(+0x12f48)[0x5629983ddf48]
[fv-az714-650:42086] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2c9ec29d90]
[fv-az714-650:42086] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2c9ec29e40]
[fv-az714-650:42086] [11] plumed(+0x131e5)[0x5629983de1e5]
[fv-az714-650:42086] *** End of error message ***
</pre>
{% endraw %}

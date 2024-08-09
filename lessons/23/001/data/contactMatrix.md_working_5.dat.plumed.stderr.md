Stderr for source:  contactMatrix.md_working_5.dat   
Download: [zipped raw stdout](contactMatrix.md_working_5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_5.dat.plumed.stderr.txt.zip) 
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
[fv-az714-382:06003] *** Process received signal ***
[fv-az714-382:06003] Signal: Aborted (6)
[fv-az714-382:06003] Signal code:  (-6)
[fv-az714-382:06003] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdedc642520]
[fv-az714-382:06003] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdedc6969fc]
[fv-az714-382:06003] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdedc642476]
[fv-az714-382:06003] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdedc6287f3]
[fv-az714-382:06003] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdedcaa2b9e]
[fv-az714-382:06003] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdedcaae20c]
[fv-az714-382:06003] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdedcaae277]
[fv-az714-382:06003] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdedcaae52b]
[fv-az714-382:06003] [ 8] plumed(+0x12f48)[0x556be2730f48]
[fv-az714-382:06003] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdedc629d90]
[fv-az714-382:06003] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdedc629e40]
[fv-az714-382:06003] [11] plumed(+0x131e5)[0x556be27311e5]
[fv-az714-382:06003] *** End of error message ***
</pre>
{% endraw %}

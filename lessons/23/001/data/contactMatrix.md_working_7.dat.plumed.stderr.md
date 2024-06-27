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
[fv-az1106-805:40083] *** Process received signal ***
[fv-az1106-805:40083] Signal: Aborted (6)
[fv-az1106-805:40083] Signal code:  (-6)
[fv-az1106-805:40083] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f397f842520]
[fv-az1106-805:40083] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f397f8969fc]
[fv-az1106-805:40083] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f397f842476]
[fv-az1106-805:40083] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f397f8287f3]
[fv-az1106-805:40083] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f397fca2b9e]
[fv-az1106-805:40083] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f397fcae20c]
[fv-az1106-805:40083] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f397fcae277]
[fv-az1106-805:40083] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f397fcae52b]
[fv-az1106-805:40083] [ 8] plumed(+0x12f48)[0x561a91752f48]
[fv-az1106-805:40083] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f397f829d90]
[fv-az1106-805:40083] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f397f829e40]
[fv-az1106-805:40083] [11] plumed(+0x131e5)[0x561a917531e5]
[fv-az1106-805:40083] *** End of error message ***
</pre>
{% endraw %}

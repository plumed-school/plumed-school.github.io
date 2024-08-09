Stderr for source:  averaging.md_working_3.dat   
Download: [zipped raw stdout](averaging.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](averaging.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ACCUMULATE LABEL=a1_denom ARG=a1_weight STRIDE=1
Maybe a missing space or a typo?
[fv-az714-382:07546] *** Process received signal ***
[fv-az714-382:07546] Signal: Aborted (6)
[fv-az714-382:07546] Signal code:  (-6)
[fv-az714-382:07546] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbba3c42520]
[fv-az714-382:07546] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbba3c969fc]
[fv-az714-382:07546] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbba3c42476]
[fv-az714-382:07546] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbba3c287f3]
[fv-az714-382:07546] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbba40a2b9e]
[fv-az714-382:07546] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbba40ae20c]
[fv-az714-382:07546] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbba40ae277]
[fv-az714-382:07546] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbba40ae52b]
[fv-az714-382:07546] [ 8] plumed(+0x12f48)[0x557247ab7f48]
[fv-az714-382:07546] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbba3c29d90]
[fv-az714-382:07546] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbba3c29e40]
[fv-az714-382:07546] [11] plumed(+0x131e5)[0x557247ab81e5]
[fv-az714-382:07546] *** End of error message ***
</pre>
{% endraw %}

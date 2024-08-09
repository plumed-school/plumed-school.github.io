Stderr for source:  Steinhardt.md_working_7.dat   
Download: [zipped raw stdout](Steinhardt.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: Q1 LABEL=q1 SPECIES=1-100 SWITCH=RATIONAL D_0=2.0 R_0=1.0 MEAN
Maybe a missing space or a typo?
[fv-az714-382:06580] *** Process received signal ***
[fv-az714-382:06580] Signal: Aborted (6)
[fv-az714-382:06580] Signal code:  (-6)
[fv-az714-382:06580] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc917a42520]
[fv-az714-382:06580] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc917a969fc]
[fv-az714-382:06580] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc917a42476]
[fv-az714-382:06580] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc917a287f3]
[fv-az714-382:06580] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc917ea2b9e]
[fv-az714-382:06580] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc917eae20c]
[fv-az714-382:06580] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc917eae277]
[fv-az714-382:06580] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc917eae52b]
[fv-az714-382:06580] [ 8] plumed(+0x12f48)[0x55e88a2a6f48]
[fv-az714-382:06580] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc917a29d90]
[fv-az714-382:06580] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc917a29e40]
[fv-az714-382:06580] [11] plumed(+0x131e5)[0x55e88a2a71e5]
[fv-az714-382:06580] *** End of error message ***
</pre>
{% endraw %}

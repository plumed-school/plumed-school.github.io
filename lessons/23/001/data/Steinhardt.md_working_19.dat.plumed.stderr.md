Stderr for source:  Steinhardt.md_working_19.dat   
Download: [zipped raw stdout](Steinhardt.md_working_19.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_19.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: Q1 LABEL=q1 SPECIES=1-100 SWITCH=RATIONAL D_0=2.0 R_0=1.0
Maybe a missing space or a typo?
[fv-az714-382:06952] *** Process received signal ***
[fv-az714-382:06952] Signal: Aborted (6)
[fv-az714-382:06952] Signal code:  (-6)
[fv-az714-382:06952] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fcd0e042520]
[fv-az714-382:06952] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fcd0e0969fc]
[fv-az714-382:06952] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fcd0e042476]
[fv-az714-382:06952] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fcd0e0287f3]
[fv-az714-382:06952] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fcd0e4a2b9e]
[fv-az714-382:06952] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fcd0e4ae20c]
[fv-az714-382:06952] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fcd0e4ae277]
[fv-az714-382:06952] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fcd0e4ae52b]
[fv-az714-382:06952] [ 8] plumed(+0x12f48)[0x55ee49bfef48]
[fv-az714-382:06952] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fcd0e029d90]
[fv-az714-382:06952] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fcd0e029e40]
[fv-az714-382:06952] [11] plumed(+0x131e5)[0x55ee49bff1e5]
[fv-az714-382:06952] *** End of error message ***
</pre>
{% endraw %}

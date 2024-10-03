Stderr for source:  averaging.md_working_8.dat   
Download: [zipped raw stdout](averaging.md_working_8.dat.plumed.stdout.txt.zip) - [zipped raw stderr](averaging.md_working_8.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: MEAN LABEL=c1_mean ARG=c1 PERIODIC=NO
Maybe a missing space or a typo?
[fv-az714-650:43504] *** Process received signal ***
[fv-az714-650:43504] Signal: Aborted (6)
[fv-az714-650:43504] Signal code:  (-6)
[fv-az714-650:43504] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f47a5a42520]
[fv-az714-650:43504] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f47a5a969fc]
[fv-az714-650:43504] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f47a5a42476]
[fv-az714-650:43504] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f47a5a287f3]
[fv-az714-650:43504] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f47a5ea2b9e]
[fv-az714-650:43504] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f47a5eae20c]
[fv-az714-650:43504] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f47a5eae277]
[fv-az714-650:43504] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f47a5eae52b]
[fv-az714-650:43504] [ 8] plumed(+0x12f48)[0x562402be5f48]
[fv-az714-650:43504] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f47a5a29d90]
[fv-az714-650:43504] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f47a5a29e40]
[fv-az714-650:43504] [11] plumed(+0x131e5)[0x562402be61e5]
[fv-az714-650:43504] *** End of error message ***
</pre>
{% endraw %}

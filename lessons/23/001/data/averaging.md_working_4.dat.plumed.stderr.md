Stderr for source:  averaging.md_working_4.dat   
Download: [zipped raw stdout](averaging.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](averaging.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ACCUMULATE LABEL=a1_denom ARG=a1_weight STRIDE=1 CLEAR=100
Maybe a missing space or a typo?
[fv-az714-650:43384] *** Process received signal ***
[fv-az714-650:43384] Signal: Aborted (6)
[fv-az714-650:43384] Signal code:  (-6)
[fv-az714-650:43384] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fee9b642520]
[fv-az714-650:43384] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fee9b6969fc]
[fv-az714-650:43384] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fee9b642476]
[fv-az714-650:43384] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fee9b6287f3]
[fv-az714-650:43384] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fee9baa2b9e]
[fv-az714-650:43384] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fee9baae20c]
[fv-az714-650:43384] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fee9baae277]
[fv-az714-650:43384] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fee9baae52b]
[fv-az714-650:43384] [ 8] plumed(+0x12f48)[0x555864daef48]
[fv-az714-650:43384] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fee9b629d90]
[fv-az714-650:43384] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fee9b629e40]
[fv-az714-650:43384] [11] plumed(+0x131e5)[0x555864daf1e5]
[fv-az714-650:43384] *** End of error message ***
</pre>
{% endraw %}

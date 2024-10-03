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
[fv-az714-650:43354] *** Process received signal ***
[fv-az714-650:43354] Signal: Aborted (6)
[fv-az714-650:43354] Signal code:  (-6)
[fv-az714-650:43354] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f94c9442520]
[fv-az714-650:43354] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f94c94969fc]
[fv-az714-650:43354] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f94c9442476]
[fv-az714-650:43354] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f94c94287f3]
[fv-az714-650:43354] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f94c98a2b9e]
[fv-az714-650:43354] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f94c98ae20c]
[fv-az714-650:43354] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f94c98ae277]
[fv-az714-650:43354] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f94c98ae52b]
[fv-az714-650:43354] [ 8] plumed(+0x12f48)[0x55d81a766f48]
[fv-az714-650:43354] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f94c9429d90]
[fv-az714-650:43354] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f94c9429e40]
[fv-az714-650:43354] [11] plumed(+0x131e5)[0x55d81a7671e5]
[fv-az714-650:43354] *** End of error message ***
</pre>
{% endraw %}

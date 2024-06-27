Stderr for source:  averaging.md_working_6.dat   
Download: [zipped raw stdout](averaging.md_working_6.dat.plumed.stdout.txt.zip) - [zipped raw stderr](averaging.md_working_6.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ACCUMULATE LABEL=a1_denom ARG=a1_weight
Maybe a missing space or a typo?
[fv-az1106-805:41608] *** Process received signal ***
[fv-az1106-805:41608] Signal: Aborted (6)
[fv-az1106-805:41608] Signal code:  (-6)
[fv-az1106-805:41608] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa4d8642520]
[fv-az1106-805:41608] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa4d86969fc]
[fv-az1106-805:41608] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa4d8642476]
[fv-az1106-805:41608] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa4d86287f3]
[fv-az1106-805:41608] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa4d8aa2b9e]
[fv-az1106-805:41608] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa4d8aae20c]
[fv-az1106-805:41608] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa4d8aae277]
[fv-az1106-805:41608] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa4d8aae52b]
[fv-az1106-805:41608] [ 8] plumed(+0x12f48)[0x55f6dbbe6f48]
[fv-az1106-805:41608] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa4d8629d90]
[fv-az1106-805:41608] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa4d8629e40]
[fv-az1106-805:41608] [11] plumed(+0x131e5)[0x55f6dbbe71e5]
[fv-az1106-805:41608] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  Path.md_working_2.dat   
Download: [zipped raw stdout](Path.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Path.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: LOWEST LABEL=p_mindist ARG=p_data
Maybe a missing space or a typo?
[fv-az1106-805:42502] *** Process received signal ***
[fv-az1106-805:42502] Signal: Aborted (6)
[fv-az1106-805:42502] Signal code:  (-6)
[fv-az1106-805:42502] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7533a42520]
[fv-az1106-805:42502] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7533a969fc]
[fv-az1106-805:42502] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7533a42476]
[fv-az1106-805:42502] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7533a287f3]
[fv-az1106-805:42502] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7533ea2b9e]
[fv-az1106-805:42502] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7533eae20c]
[fv-az1106-805:42502] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7533eae277]
[fv-az1106-805:42502] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7533eae52b]
[fv-az1106-805:42502] [ 8] plumed(+0x12f48)[0x5558308fcf48]
[fv-az1106-805:42502] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7533a29d90]
[fv-az1106-805:42502] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7533a29e40]
[fv-az1106-805:42502] [11] plumed(+0x131e5)[0x5558308fd1e5]
[fv-az1106-805:42502] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  Tasks.md_working_3.dat   
Download: [zipped raw stdout](Tasks.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tasks.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: ONES LABEL=ones SIZE=100
Maybe a missing space or a typo?
[fv-az1106-805:40202] *** Process received signal ***
[fv-az1106-805:40202] Signal: Aborted (6)
[fv-az1106-805:40202] Signal code:  (-6)
[fv-az1106-805:40202] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1958a42520]
[fv-az1106-805:40202] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1958a969fc]
[fv-az1106-805:40202] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1958a42476]
[fv-az1106-805:40202] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1958a287f3]
[fv-az1106-805:40202] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1958ea2b9e]
[fv-az1106-805:40202] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1958eae20c]
[fv-az1106-805:40202] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1958eae277]
[fv-az1106-805:40202] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1958eae52b]
[fv-az1106-805:40202] [ 8] plumed(+0x12f48)[0x564663377f48]
[fv-az1106-805:40202] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1958a29d90]
[fv-az1106-805:40202] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1958a29e40]
[fv-az1106-805:40202] [11] plumed(+0x131e5)[0x5646633781e5]
[fv-az1106-805:40202] *** End of error message ***
</pre>
{% endraw %}

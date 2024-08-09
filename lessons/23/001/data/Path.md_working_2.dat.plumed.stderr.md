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
[fv-az714-382:08541] *** Process received signal ***
[fv-az714-382:08541] Signal: Aborted (6)
[fv-az714-382:08541] Signal code:  (-6)
[fv-az714-382:08541] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4a2e842520]
[fv-az714-382:08541] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4a2e8969fc]
[fv-az714-382:08541] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4a2e842476]
[fv-az714-382:08541] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4a2e8287f3]
[fv-az714-382:08541] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4a2eca2b9e]
[fv-az714-382:08541] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4a2ecae20c]
[fv-az714-382:08541] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4a2ecae277]
[fv-az714-382:08541] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4a2ecae52b]
[fv-az714-382:08541] [ 8] plumed(+0x12f48)[0x561be0aadf48]
[fv-az714-382:08541] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4a2e829d90]
[fv-az714-382:08541] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4a2e829e40]
[fv-az714-382:08541] [11] plumed(+0x131e5)[0x561be0aae1e5]
[fv-az714-382:08541] *** End of error message ***
</pre>
{% endraw %}

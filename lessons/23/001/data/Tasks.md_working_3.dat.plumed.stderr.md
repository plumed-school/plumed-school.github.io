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
[fv-az714-650:42040] *** Process received signal ***
[fv-az714-650:42040] Signal: Aborted (6)
[fv-az714-650:42040] Signal code:  (-6)
[fv-az714-650:42040] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f598c842520]
[fv-az714-650:42040] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f598c8969fc]
[fv-az714-650:42040] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f598c842476]
[fv-az714-650:42040] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f598c8287f3]
[fv-az714-650:42040] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f598cca2b9e]
[fv-az714-650:42040] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f598ccae20c]
[fv-az714-650:42040] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f598ccae277]
[fv-az714-650:42040] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f598ccae52b]
[fv-az714-650:42040] [ 8] plumed(+0x12f48)[0x55668d4ecf48]
[fv-az714-650:42040] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f598c829d90]
[fv-az714-650:42040] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f598c829e40]
[fv-az714-650:42040] [11] plumed(+0x131e5)[0x55668d4ed1e5]
[fv-az714-650:42040] *** End of error message ***
</pre>
{% endraw %}

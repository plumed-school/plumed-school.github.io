Stderr for source:  averaging.md_working_9.dat   
Download: [zipped raw stdout](averaging.md_working_9.dat.plumed.stdout.txt.zip) - [zipped raw stderr](averaging.md_working_9.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=r1g ARG=r1.bias
Maybe a missing space or a typo?
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
[fv-az714-650:43538] *** Process received signal ***
[fv-az714-650:43538] Signal: Aborted (6)
[fv-az714-650:43538] Signal code:  (-6)
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=r1g ARG=r1.bias
Maybe a missing space or a typo?
[fv-az714-650:43538] [ 0] [fv-az714-650:43539] *** Process received signal ***
[fv-az714-650:43539] Signal: Aborted (6)
[fv-az714-650:43539] Signal code:  (-6)
[fv-az714-650:43539] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f863d442520]
[fv-az714-650:43538] [ 1] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4ae6442520]
[fv-az714-650:43539] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f863d4969fc]
[fv-az714-650:43538] [ 2] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4ae64969fc]
[fv-az714-650:43539] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4ae6442476]
[fv-az714-650:43539] [ 3] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f863d442476]
[fv-az714-650:43538] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4ae64287f3]
[fv-az714-650:43539] [ 4] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f863d4287f3]
[fv-az714-650:43538] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f4ae68a2b9e]
[fv-az714-650:43539] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f4ae68ae20c]
[fv-az714-650:43539] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f863d8a2b9e]
[fv-az714-650:43538] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f4ae68ae277]
[fv-az714-650:43539] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f863d8ae20c]
[fv-az714-650:43538] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f4ae68ae52b]
[fv-az714-650:43539] [ 8] plumed(+0x12f48)[0x5611177a5f48]
[fv-az714-650:43539] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4ae6429d90]
[fv-az714-650:43539] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4ae6429e40]
[fv-az714-650:43539] [11] plumed(+0x131e5)[0x5611177a61e5]
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f863d8ae277]
[fv-az714-650:43538] [ 7] [fv-az714-650:43539] *** End of error message ***
/lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f863d8ae52b]
[fv-az714-650:43538] [ 8] plumed(+0x12f48)[0x558409264f48]
[fv-az714-650:43538] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f863d429d90]
[fv-az714-650:43538] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f863d429e40]
[fv-az714-650:43538] [11] plumed(+0x131e5)[0x5584092651e5]
[fv-az714-650:43538] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az714-650 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

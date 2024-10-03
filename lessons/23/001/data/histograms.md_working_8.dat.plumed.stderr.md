Stderr for source:  histograms.md_working_8.dat   
Download: [zipped raw stdout](histograms.md_working_8.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_8.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
terminate called after throwing an instance of '  what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=d1c ARG=d1
Maybe a missing space or a typo?
PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=d1c ARG=d1
Maybe a missing space or a typo?
[fv-az714-650:43817] *** Process received signal ***
[fv-az714-650:43818] *** Process received signal ***
[fv-az714-650:43818] Signal: Aborted (6)
[fv-az714-650:43818] Signal code:  (-6)
[fv-az714-650:43817] Signal: Aborted (6)
[fv-az714-650:43817] Signal code:  (-6)
[fv-az714-650:43818] [ 0] [fv-az714-650:43817] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe822442520]
[fv-az714-650:43818] [ 1] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8e09242520]
[fv-az714-650:43817] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe8224969fc]
[fv-az714-650:43818] [ 2] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8e092969fc]
[fv-az714-650:43817] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8e09242476]
[fv-az714-650:43817] [ 3] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe822442476]
[fv-az714-650:43818] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8e092287f3]
[fv-az714-650:43817] [ 4] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe8224287f3]
[fv-az714-650:43818] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8e096a2b9e]
[fv-az714-650:43817] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8e096ae20c]
[fv-az714-650:43817] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe8228a2b9e]
[fv-az714-650:43818] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8e096ae277]
[fv-az714-650:43817] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8e096ae52b]
[fv-az714-650:43817] [ 8] plumed(+0x12f48)[0x559a6b7f7f48]
[fv-az714-650:43817] [ 9] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe8228ae20c]
[fv-az714-650:43818] [ 6] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8e09229d90]
[fv-az714-650:43817] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8e09229e40]
[fv-az714-650:43817] [11] plumed(+0x131e5)[0x559a6b7f81e5]
[fv-az714-650:43817] *** End of error message ***
/lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe8228ae277]
[fv-az714-650:43818] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe8228ae52b]
[fv-az714-650:43818] [ 8] plumed(+0x12f48)[0x558a9c44af48]
[fv-az714-650:43818] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe822429d90]
[fv-az714-650:43818] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe822429e40]
[fv-az714-650:43818] [11] plumed(+0x131e5)[0x558a9c44b1e5]
[fv-az714-650:43818] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az714-650 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

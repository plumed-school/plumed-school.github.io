Stderr for source:  histograms.md_working_8.dat   
Download: [zipped raw stdout](histograms.md_working_8.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_8.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=d1c ARG=d1
Maybe a missing space or a typo?
[fv-az1106-805:41981] *** Process received signal ***
[fv-az1106-805:41981] Signal: Aborted (6)
[fv-az1106-805:41981] Signal code:  (-6)
[fv-az1106-805:41981] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1705442520]
[fv-az1106-805:41981] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f17054969fc]
[fv-az1106-805:41981] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1705442476]
[fv-az1106-805:41981] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f17054287f3]
[fv-az1106-805:41981] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f17058a2b9e]
[fv-az1106-805:41981] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f17058ae20c]
[fv-az1106-805:41981] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f17058ae277]
[fv-az1106-805:41981] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f17058ae52b]
[fv-az1106-805:41981] [ 8] plumed(+0x12f48)[0x559f74a97f48]
[fv-az1106-805:41981] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1705429d90]
[fv-az1106-805:41981] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1705429e40]
[fv-az1106-805:41981] [11] plumed(+0x131e5)[0x559f74a981e5]
[fv-az1106-805:41981] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=d1c ARG=d1
Maybe a missing space or a typo?
[fv-az1106-805:41980] *** Process received signal ***
[fv-az1106-805:41980] Signal: Aborted (6)
[fv-az1106-805:41980] Signal code:  (-6)
[fv-az1106-805:41980] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc76a042520]
[fv-az1106-805:41980] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc76a0969fc]
[fv-az1106-805:41980] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc76a042476]
[fv-az1106-805:41980] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc76a0287f3]
[fv-az1106-805:41980] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc76a4a2b9e]
[fv-az1106-805:41980] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc76a4ae20c]
[fv-az1106-805:41980] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc76a4ae277]
[fv-az1106-805:41980] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc76a4ae52b]
[fv-az1106-805:41980] [ 8] plumed(+0x12f48)[0x5653a3ed0f48]
[fv-az1106-805:41980] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc76a029d90]
[fv-az1106-805:41980] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc76a029e40]
[fv-az1106-805:41980] [11] plumed(+0x131e5)[0x5653a3ed11e5]
[fv-az1106-805:41980] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1106-805 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

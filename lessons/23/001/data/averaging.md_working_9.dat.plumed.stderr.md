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
[fv-az1106-805:41703] *** Process received signal ***
[fv-az1106-805:41703] Signal: Aborted (6)
[fv-az1106-805:41703] Signal code:  (-6)
[fv-az1106-805:41703] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc803a42520]
[fv-az1106-805:41703] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc803a969fc]
[fv-az1106-805:41703] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc803a42476]
[fv-az1106-805:41703] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc803a287f3]
[fv-az1106-805:41703] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc803ea2b9e]
[fv-az1106-805:41703] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc803eae20c]
[fv-az1106-805:41703] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc803eae277]
[fv-az1106-805:41703] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc803eae52b]
[fv-az1106-805:41703] [ 8] plumed(+0x12f48)[0x55d0a9fc0f48]
[fv-az1106-805:41703] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc803a29d90]
[fv-az1106-805:41703] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc803a29e40]
[fv-az1106-805:41703] [11] plumed(+0x131e5)[0x55d0a9fc11e5]
[fv-az1106-805:41703] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=r1g ARG=r1.bias
Maybe a missing space or a typo?
[fv-az1106-805:41702] *** Process received signal ***
[fv-az1106-805:41702] Signal: Aborted (6)
[fv-az1106-805:41702] Signal code:  (-6)
[fv-az1106-805:41702] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1a3f842520]
[fv-az1106-805:41702] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1a3f8969fc]
[fv-az1106-805:41702] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1a3f842476]
[fv-az1106-805:41702] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1a3f8287f3]
[fv-az1106-805:41702] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1a3fca2b9e]
[fv-az1106-805:41702] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1a3fcae20c]
[fv-az1106-805:41702] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1a3fcae277]
[fv-az1106-805:41702] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1a3fcae52b]
[fv-az1106-805:41702] [ 8] plumed(+0x12f48)[0x55bfd110df48]
[fv-az1106-805:41702] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1a3f829d90]
[fv-az1106-805:41702] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1a3f829e40]
[fv-az1106-805:41702] [11] plumed(+0x131e5)[0x55bfd110e1e5]
[fv-az1106-805:41702] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az1106-805 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

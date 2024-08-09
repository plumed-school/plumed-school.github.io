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
[fv-az714-382:07733] *** Process received signal ***
[fv-az714-382:07733] Signal: Aborted (6)
[fv-az714-382:07733] Signal code:  (-6)
[fv-az714-382:07733] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7f0c042520]
[fv-az714-382:07733] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7f0c0969fc]
[fv-az714-382:07733] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7f0c042476]
[fv-az714-382:07733] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7f0c0287f3]
[fv-az714-382:07733] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7f0c4a2b9e]
[fv-az714-382:07733] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7f0c4ae20c]
[fv-az714-382:07733] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7f0c4ae277]
[fv-az714-382:07733] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7f0c4ae52b]
[fv-az714-382:07733] [ 8] plumed(+0x12f48)[0x561ae097af48]
[fv-az714-382:07733] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7f0c029d90]
[fv-az714-382:07733] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7f0c029e40]
[fv-az714-382:07733] [11] plumed(+0x131e5)[0x561ae097b1e5]
[fv-az714-382:07733] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=r1g ARG=r1.bias
Maybe a missing space or a typo?
[fv-az714-382:07734] *** Process received signal ***
[fv-az714-382:07734] Signal: Aborted (6)
[fv-az714-382:07734] Signal code:  (-6)
[fv-az714-382:07734] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa65e642520]
[fv-az714-382:07734] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa65e6969fc]
[fv-az714-382:07734] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa65e642476]
[fv-az714-382:07734] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa65e6287f3]
[fv-az714-382:07734] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa65eaa2b9e]
[fv-az714-382:07734] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa65eaae20c]
[fv-az714-382:07734] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa65eaae277]
[fv-az714-382:07734] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa65eaae52b]
[fv-az714-382:07734] [ 8] plumed(+0x12f48)[0x562a6a3e7f48]
[fv-az714-382:07734] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa65e629d90]
[fv-az714-382:07734] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa65e629e40]
[fv-az714-382:07734] [11] plumed(+0x131e5)[0x562a6a3e81e5]
[fv-az714-382:07734] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 0 with PID 0 on node fv-az714-382 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

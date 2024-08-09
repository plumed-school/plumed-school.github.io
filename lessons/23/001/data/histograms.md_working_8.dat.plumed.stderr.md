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
[fv-az714-382:08014] *** Process received signal ***
[fv-az714-382:08014] Signal: Aborted (6)
[fv-az714-382:08014] Signal code:  (-6)
[fv-az714-382:08014] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1d40842520]
[fv-az714-382:08014] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1d408969fc]
[fv-az714-382:08014] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1d40842476]
[fv-az714-382:08014] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1d408287f3]
[fv-az714-382:08014] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1d40ca2b9e]
[fv-az714-382:08014] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1d40cae20c]
[fv-az714-382:08014] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1d40cae277]
[fv-az714-382:08014] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1d40cae52b]
[fv-az714-382:08014] [ 8] plumed(+0x12f48)[0x562d81938f48]
[fv-az714-382:08014] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1d40829d90]
[fv-az714-382:08014] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1d40829e40]
[fv-az714-382:08014] [11] plumed(+0x131e5)[0x562d819391e5]
[fv-az714-382:08014] *** End of error message ***
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: GATHER_REPLICAS LABEL=d1c ARG=d1
Maybe a missing space or a typo?
[fv-az714-382:08015] *** Process received signal ***
[fv-az714-382:08015] Signal: Aborted (6)
[fv-az714-382:08015] Signal code:  (-6)
[fv-az714-382:08015] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3ac6042520]
[fv-az714-382:08015] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3ac60969fc]
[fv-az714-382:08015] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3ac6042476]
[fv-az714-382:08015] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3ac60287f3]
[fv-az714-382:08015] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3ac64a2b9e]
[fv-az714-382:08015] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3ac64ae20c]
[fv-az714-382:08015] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3ac64ae277]
[fv-az714-382:08015] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3ac64ae52b]
[fv-az714-382:08015] [ 8] plumed(+0x12f48)[0x55ab02df9f48]
[fv-az714-382:08015] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3ac6029d90]
[fv-az714-382:08015] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3ac6029e40]
[fv-az714-382:08015] [11] plumed(+0x131e5)[0x55ab02dfa1e5]
[fv-az714-382:08015] *** End of error message ***
--------------------------------------------------------------------------
Primary job  terminated normally, but 1 process returned
a non-zero exit code. Per user-direction, the job has been aborted.
--------------------------------------------------------------------------
--------------------------------------------------------------------------
mpirun noticed that process rank 1 with PID 0 on node fv-az714-382 exited on signal 6 (Aborted).
--------------------------------------------------------------------------
</pre>
{% endraw %}

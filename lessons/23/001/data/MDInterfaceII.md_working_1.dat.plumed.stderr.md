Stderr for source:  MDInterfaceII.md_working_1.dat   
Download: [zipped raw stdout](MDInterfaceII.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MDInterfaceII.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1063) void PLMD::PlumedMain::readInputLine(const std::string&, const bool&)
+++ assertion failed: citations.empty()
[runnervm76f27:04160] *** Process received signal ***
[runnervm76f27:04160] Signal: Aborted (6)
[runnervm76f27:04160] Signal code:  (-6)
[runnervm76f27:04160] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2e9c445330]
[runnervm76f27:04160] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2e9c49ec0c]
[runnervm76f27:04160] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2e9c44527e]
[runnervm76f27:04160] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2e9c4288ff]
[runnervm76f27:04160] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2e9c8a5ff5]
[runnervm76f27:04160] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2e9c8bb0da]
[runnervm76f27:04160] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2e9c8a5a55]
[runnervm76f27:04160] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2e9c8a5a6f]
[runnervm76f27:04160] [ 8] plumed(+0x146dd)[0x5578b6d2c6dd]
[runnervm76f27:04160] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2e9c42a1ca]
[runnervm76f27:04160] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2e9c42a28b]
[runnervm76f27:04160] [11] plumed(+0x15365)[0x5578b6d2d365]
[runnervm76f27:04160] *** End of error message ***
</pre>
{% endraw %}

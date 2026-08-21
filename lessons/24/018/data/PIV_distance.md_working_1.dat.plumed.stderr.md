Stderr for source:  PIV_distance.md_working_1.dat   
Download: [zipped raw stdout](PIV_distance.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](PIV_distance.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1546) FILE* PLMD::PlumedMain::fopen(const char*, const char*)
+++ assertion failed: fp
file Liq.pdb cannot be found
[runnervm76f27:04606] *** Process received signal ***
[runnervm76f27:04606] Signal: Aborted (6)
[runnervm76f27:04606] Signal code:  (-6)
[runnervm76f27:04606] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc8ae045330]
[runnervm76f27:04606] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc8ae09ec0c]
[runnervm76f27:04606] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc8ae04527e]
[runnervm76f27:04606] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc8ae0288ff]
[runnervm76f27:04606] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc8ae4a5ff5]
[runnervm76f27:04606] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc8ae4bb0da]
[runnervm76f27:04606] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc8ae4a5a55]
[runnervm76f27:04606] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc8ae4a5a6f]
[runnervm76f27:04606] [ 8] plumed(+0x146dd)[0x555bfcf9f6dd]
[runnervm76f27:04606] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc8ae02a1ca]
[runnervm76f27:04606] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc8ae02a28b]
[runnervm76f27:04606] [11] plumed(+0x15365)[0x555bfcfa0365]
[runnervm76f27:04606] *** End of error message ***
</pre>
{% endraw %}

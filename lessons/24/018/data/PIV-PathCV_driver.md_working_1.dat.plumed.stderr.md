Stderr for source:  PIV-PathCV_driver.md_working_1.dat   
Download: [zipped raw stdout](PIV-PathCV_driver.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](PIV-PathCV_driver.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1546) FILE* PLMD::PlumedMain::fopen(const char*, const char*)
+++ assertion failed: fp
file Liq.pdb cannot be found
[runnervm76f27:04664] *** Process received signal ***
[runnervm76f27:04664] Signal: Aborted (6)
[runnervm76f27:04664] Signal code:  (-6)
[runnervm76f27:04664] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ff119245330]
[runnervm76f27:04664] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ff11929ec0c]
[runnervm76f27:04664] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ff11924527e]
[runnervm76f27:04664] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ff1192288ff]
[runnervm76f27:04664] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ff1196a5ff5]
[runnervm76f27:04664] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ff1196bb0da]
[runnervm76f27:04664] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ff1196a5a55]
[runnervm76f27:04664] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ff1196a5a6f]
[runnervm76f27:04664] [ 8] plumed(+0x146dd)[0x55b6179626dd]
[runnervm76f27:04664] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ff11922a1ca]
[runnervm76f27:04664] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ff11922a28b]
[runnervm76f27:04664] [11] plumed(+0x15365)[0x55b617963365]
[runnervm76f27:04664] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  PIV_distance.md_working_1.dat   
Download: [zipped raw stdout](PIV_distance.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](PIV_distance.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1545) FILE* PLMD::PlumedMain::fopen(const char*, const char*)
+++ assertion failed: fp
file Liq.pdb cannot be found
[runnervm76f27:04623] *** Process received signal ***
[runnervm76f27:04623] Signal: Aborted (6)
[runnervm76f27:04623] Signal code:  (-6)
[runnervm76f27:04623] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fd177645330]
[runnervm76f27:04623] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fd17769ec0c]
[runnervm76f27:04623] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fd17764527e]
[runnervm76f27:04623] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fd1776288ff]
[runnervm76f27:04623] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fd177aa5ff5]
[runnervm76f27:04623] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fd177abb0da]
[runnervm76f27:04623] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fd177aa5a55]
[runnervm76f27:04623] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fd177aa5a6f]
[runnervm76f27:04623] [ 8] plumed_master(+0x146dd)[0x55bf44f2f6dd]
[runnervm76f27:04623] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fd17762a1ca]
[runnervm76f27:04623] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fd17762a28b]
[runnervm76f27:04623] [11] plumed_master(+0x15365)[0x55bf44f30365]
[runnervm76f27:04623] *** End of error message ***
</pre>
{% endraw %}

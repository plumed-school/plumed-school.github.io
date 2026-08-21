Stderr for source:  PIV-PathCV_driver.md_working_1.dat   
Download: [zipped raw stdout](PIV-PathCV_driver.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](PIV-PathCV_driver.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:1545) FILE* PLMD::PlumedMain::fopen(const char*, const char*)
+++ assertion failed: fp
file Liq.pdb cannot be found
[runnervm76f27:04680] *** Process received signal ***
[runnervm76f27:04680] Signal: Aborted (6)
[runnervm76f27:04680] Signal code:  (-6)
[runnervm76f27:04680] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f294aa45330]
[runnervm76f27:04680] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f294aa9ec0c]
[runnervm76f27:04680] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f294aa4527e]
[runnervm76f27:04680] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f294aa288ff]
[runnervm76f27:04680] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f294aea5ff5]
[runnervm76f27:04680] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f294aebb0da]
[runnervm76f27:04680] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f294aea5a55]
[runnervm76f27:04680] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f294aea5a6f]
[runnervm76f27:04680] [ 8] plumed_master(+0x146dd)[0x55da7cb246dd]
[runnervm76f27:04680] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f294aa2a1ca]
[runnervm76f27:04680] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f294aa2a28b]
[runnervm76f27:04680] [11] plumed_master(+0x15365)[0x55da7cb25365]
[runnervm76f27:04680] *** End of error message ***
</pre>
{% endraw %}

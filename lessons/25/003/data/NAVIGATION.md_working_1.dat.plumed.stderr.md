Stderr for source:  NAVIGATION.md_working_1.dat   
Download: [zipped raw stdout](NAVIGATION.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](NAVIGATION.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'std::runtime_error'
what():  Can not use metatomic action without the corresponding libraries.
Make sure to configure with `--enable-libmetatomic --enable-libtorch` and that the corresponding libraries are found
[runnervm76f27:04192] *** Process received signal ***
[runnervm76f27:04192] Signal: Aborted (6)
[runnervm76f27:04192] Signal code:  (-6)
[runnervm76f27:04192] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa3d5845330]
[runnervm76f27:04192] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa3d589ec0c]
[runnervm76f27:04192] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa3d584527e]
[runnervm76f27:04192] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa3d58288ff]
[runnervm76f27:04192] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa3d5ca5ff5]
[runnervm76f27:04192] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa3d5cbb0da]
[runnervm76f27:04192] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa3d5ca5a55]
[runnervm76f27:04192] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa3d5ca5a6f]
[runnervm76f27:04192] [ 8] plumed(+0x146dd)[0x55f325c406dd]
[runnervm76f27:04192] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa3d582a1ca]
[runnervm76f27:04192] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa3d582a28b]
[runnervm76f27:04192] [11] plumed(+0x15365)[0x55f325c41365]
[runnervm76f27:04192] *** End of error message ***
</pre>
{% endraw %}

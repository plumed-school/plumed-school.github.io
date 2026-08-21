Stderr for source:  NAVIGATION.md_working_1.dat   
Download: [zipped raw stdout](NAVIGATION.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](NAVIGATION.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'std::runtime_error'
what():  Can not use metatomic action without the corresponding libraries.
Make sure to configure with `--enable-libmetatomic --enable-libtorch` and that the corresponding libraries are found
[runnervm76f27:04207] *** Process received signal ***
[runnervm76f27:04207] Signal: Aborted (6)
[runnervm76f27:04207] Signal code:  (-6)
[runnervm76f27:04207] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fbc77e45330]
[runnervm76f27:04207] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fbc77e9ec0c]
[runnervm76f27:04207] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fbc77e4527e]
[runnervm76f27:04207] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fbc77e288ff]
[runnervm76f27:04207] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fbc782a5ff5]
[runnervm76f27:04207] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fbc782bb0da]
[runnervm76f27:04207] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fbc782a5a55]
[runnervm76f27:04207] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fbc782a5a6f]
[runnervm76f27:04207] [ 8] plumed_master(+0x146dd)[0x55e6909516dd]
[runnervm76f27:04207] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fbc77e2a1ca]
[runnervm76f27:04207] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fbc77e2a28b]
[runnervm76f27:04207] [11] plumed_master(+0x15365)[0x55e690952365]
[runnervm76f27:04207] *** End of error message ***
</pre>
{% endraw %}

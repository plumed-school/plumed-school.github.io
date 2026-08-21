Stderr for source:  input.md_working_2.dat   
Download: [zipped raw stdout](input.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](input.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "MAZE_OPT_ANNEALING" is not known.
[runnervm76f27:04463] *** Process received signal ***
[runnervm76f27:04463] Signal: Aborted (6)
[runnervm76f27:04463] Signal code:  (-6)
[runnervm76f27:04463] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f7b7e645330]
[runnervm76f27:04463] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f7b7e69ec0c]
[runnervm76f27:04463] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f7b7e64527e]
[runnervm76f27:04463] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f7b7e6288ff]
[runnervm76f27:04463] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f7b7eaa5ff5]
[runnervm76f27:04463] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f7b7eabb0da]
[runnervm76f27:04463] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f7b7eaa5a55]
[runnervm76f27:04463] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f7b7eaa5a6f]
[runnervm76f27:04463] [ 8] plumed_master(+0x146dd)[0x55bd091236dd]
[runnervm76f27:04463] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f7b7e62a1ca]
[runnervm76f27:04463] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f7b7e62a28b]
[runnervm76f27:04463] [11] plumed_master(+0x15365)[0x55bd09124365]
[runnervm76f27:04463] *** End of error message ***
</pre>
{% endraw %}

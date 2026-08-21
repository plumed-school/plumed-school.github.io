Stderr for source:  input.md_working_3.dat   
Download: [zipped raw stdout](input.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](input.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "MAZE_OPT_ANNEALING" is not known.
[runnervm76f27:04509] *** Process received signal ***
[runnervm76f27:04509] Signal: Aborted (6)
[runnervm76f27:04509] Signal code:  (-6)
[runnervm76f27:04509] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0cc6445330]
[runnervm76f27:04509] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0cc649ec0c]
[runnervm76f27:04509] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0cc644527e]
[runnervm76f27:04509] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0cc64288ff]
[runnervm76f27:04509] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0cc68a5ff5]
[runnervm76f27:04509] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0cc68bb0da]
[runnervm76f27:04509] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0cc68a5a55]
[runnervm76f27:04509] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0cc68a5a6f]
[runnervm76f27:04509] [ 8] plumed_master(+0x146dd)[0x5582ac9a26dd]
[runnervm76f27:04509] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0cc642a1ca]
[runnervm76f27:04509] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0cc642a28b]
[runnervm76f27:04509] [11] plumed_master(+0x15365)[0x5582ac9a3365]
[runnervm76f27:04509] *** End of error message ***
</pre>
{% endraw %}

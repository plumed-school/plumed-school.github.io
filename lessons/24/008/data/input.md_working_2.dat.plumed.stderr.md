Stderr for source:  input.md_working_2.dat   
Download: [zipped raw stdout](input.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](input.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "MAZE_OPT_ANNEALING" is not known.
[runnervm76f27:04448] *** Process received signal ***
[runnervm76f27:04448] Signal: Aborted (6)
[runnervm76f27:04448] Signal code:  (-6)
[runnervm76f27:04448] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6d7fc45330]
[runnervm76f27:04448] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6d7fc9ec0c]
[runnervm76f27:04448] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6d7fc4527e]
[runnervm76f27:04448] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6d7fc288ff]
[runnervm76f27:04448] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6d800a5ff5]
[runnervm76f27:04448] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6d800bb0da]
[runnervm76f27:04448] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6d800a5a55]
[runnervm76f27:04448] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6d800a5a6f]
[runnervm76f27:04448] [ 8] plumed(+0x146dd)[0x55ec4efab6dd]
[runnervm76f27:04448] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6d7fc2a1ca]
[runnervm76f27:04448] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6d7fc2a28b]
[runnervm76f27:04448] [11] plumed(+0x15365)[0x55ec4efac365]
[runnervm76f27:04448] *** End of error message ***
</pre>
{% endraw %}

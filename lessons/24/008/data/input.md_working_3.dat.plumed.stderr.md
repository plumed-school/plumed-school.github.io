Stderr for source:  input.md_working_3.dat   
Download: [zipped raw stdout](input.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](input.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
Action "MAZE_OPT_ANNEALING" is not known.
[runnervm76f27:04493] *** Process received signal ***
[runnervm76f27:04493] Signal: Aborted (6)
[runnervm76f27:04493] Signal code:  (-6)
[runnervm76f27:04493] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f567fe45330]
[runnervm76f27:04493] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f567fe9ec0c]
[runnervm76f27:04493] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f567fe4527e]
[runnervm76f27:04493] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f567fe288ff]
[runnervm76f27:04493] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f56802a5ff5]
[runnervm76f27:04493] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f56802bb0da]
[runnervm76f27:04493] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f56802a5a55]
[runnervm76f27:04493] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f56802a5a6f]
[runnervm76f27:04493] [ 8] plumed(+0x146dd)[0x5568b72e76dd]
[runnervm76f27:04493] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f567fe2a1ca]
[runnervm76f27:04493] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f567fe2a28b]
[runnervm76f27:04493] [11] plumed(+0x15365)[0x5568b72e8365]
[runnervm76f27:04493] *** End of error message ***
</pre>
{% endraw %}

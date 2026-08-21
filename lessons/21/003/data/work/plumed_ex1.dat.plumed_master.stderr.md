Stderr for source:  work/plumed_ex1.dat   
Download: [zipped raw stdout](plumed_ex1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @24 : keyword ARG is compulsory for this action
[runnervm76f27:05811] *** Process received signal ***
[runnervm76f27:05811] Signal: Aborted (6)
[runnervm76f27:05811] Signal code:  (-6)
[runnervm76f27:05811] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe477e45330]
[runnervm76f27:05811] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe477e9ec0c]
[runnervm76f27:05811] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe477e4527e]
[runnervm76f27:05811] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe477e288ff]
[runnervm76f27:05811] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe4782a5ff5]
[runnervm76f27:05811] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe4782bb0da]
[runnervm76f27:05811] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe4782a5a55]
[runnervm76f27:05811] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe4782a5a6f]
[runnervm76f27:05811] [ 8] plumed_master(+0x146dd)[0x5629f2df36dd]
[runnervm76f27:05811] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe477e2a1ca]
[runnervm76f27:05811] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe477e2a28b]
[runnervm76f27:05811] [11] plumed_master(+0x15365)[0x5629f2df4365]
[runnervm76f27:05811] *** End of error message ***
</pre>
{% endraw %}

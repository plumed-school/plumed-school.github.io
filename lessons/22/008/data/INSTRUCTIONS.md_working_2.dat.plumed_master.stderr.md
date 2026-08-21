Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DFSCLUSTERING with label dfs : keyword ARG is compulsory for this action
[runnervm76f27:06035] *** Process received signal ***
[runnervm76f27:06035] Signal: Aborted (6)
[runnervm76f27:06035] Signal code:  (-6)
[runnervm76f27:06035] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0c3ae45330]
[runnervm76f27:06035] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f0c3ae9ec0c]
[runnervm76f27:06035] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f0c3ae4527e]
[runnervm76f27:06035] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f0c3ae288ff]
[runnervm76f27:06035] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0c3b2a5ff5]
[runnervm76f27:06035] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0c3b2bb0da]
[runnervm76f27:06035] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0c3b2a5a55]
[runnervm76f27:06035] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0c3b2a5a6f]
[runnervm76f27:06035] [ 8] plumed_master(+0x146dd)[0x55d6be3666dd]
[runnervm76f27:06035] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f0c3ae2a1ca]
[runnervm76f27:06035] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f0c3ae2a28b]
[runnervm76f27:06035] [11] plumed_master(+0x15365)[0x55d6be367365]
[runnervm76f27:06035] *** End of error message ***
</pre>
{% endraw %}

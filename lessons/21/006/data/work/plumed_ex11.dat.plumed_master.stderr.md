Stderr for source:  work/plumed_ex11.dat   
Download: [zipped raw stdout](plumed_ex11.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex11.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @73 : keyword ARG is compulsory for this action
[runnervm76f27:05867] *** Process received signal ***
[runnervm76f27:05867] Signal: Aborted (6)
[runnervm76f27:05867] Signal code:  (-6)
[runnervm76f27:05867] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4817a45330]
[runnervm76f27:05867] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4817a9ec0c]
[runnervm76f27:05867] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4817a4527e]
[runnervm76f27:05867] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4817a288ff]
[runnervm76f27:05867] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4817ea5ff5]
[runnervm76f27:05867] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4817ebb0da]
[runnervm76f27:05867] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4817ea5a55]
[runnervm76f27:05867] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4817ea5a6f]
[runnervm76f27:05867] [ 8] plumed_master(+0x146dd)[0x55c5ac3ba6dd]
[runnervm76f27:05867] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4817a2a1ca]
[runnervm76f27:05867] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4817a2a28b]
[runnervm76f27:05867] [11] plumed_master(+0x15365)[0x55c5ac3bb365]
[runnervm76f27:05867] *** End of error message ***
</pre>
{% endraw %}

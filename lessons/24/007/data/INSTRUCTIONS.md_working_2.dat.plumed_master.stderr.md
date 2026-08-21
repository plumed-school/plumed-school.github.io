Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[runnervm76f27:05332] *** Process received signal ***
[runnervm76f27:05332] Signal: Aborted (6)
[runnervm76f27:05332] Signal code:  (-6)
[runnervm76f27:05332] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe6de645330]
[runnervm76f27:05332] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe6de69ec0c]
[runnervm76f27:05332] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe6de64527e]
[runnervm76f27:05332] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe6de6288ff]
[runnervm76f27:05332] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe6deaa5ff5]
[runnervm76f27:05332] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe6deabb0da]
[runnervm76f27:05332] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe6deaa5a55]
[runnervm76f27:05332] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe6deaa5a6f]
[runnervm76f27:05332] [ 8] plumed_master(+0x146dd)[0x55c58c4576dd]
[runnervm76f27:05332] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe6de62a1ca]
[runnervm76f27:05332] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe6de62a28b]
[runnervm76f27:05332] [11] plumed_master(+0x15365)[0x55c58c458365]
[runnervm76f27:05332] *** End of error message ***
</pre>
{% endraw %}

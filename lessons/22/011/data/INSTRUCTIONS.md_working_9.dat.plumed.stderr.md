Stderr for source:  INSTRUCTIONS.md_working_9.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_9.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_9.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label dist : could not find file named colvar_reweight.data
[runnervm76f27:05509] *** Process received signal ***
[runnervm76f27:05509] Signal: Aborted (6)
[runnervm76f27:05509] Signal code:  (-6)
[runnervm76f27:05509] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2796a45330]
[runnervm76f27:05509] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2796a9ec0c]
[runnervm76f27:05509] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2796a4527e]
[runnervm76f27:05509] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2796a288ff]
[runnervm76f27:05509] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2796ea5ff5]
[runnervm76f27:05509] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2796ebb0da]
[runnervm76f27:05509] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2796ea5a55]
[runnervm76f27:05509] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2796ea5a6f]
[runnervm76f27:05509] [ 8] plumed(+0x146dd)[0x5618399576dd]
[runnervm76f27:05509] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2796a2a1ca]
[runnervm76f27:05509] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2796a2a28b]
[runnervm76f27:05509] [11] plumed(+0x15365)[0x561839958365]
[runnervm76f27:05509] *** End of error message ***
</pre>
{% endraw %}

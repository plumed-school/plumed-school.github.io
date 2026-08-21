Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : keyword SIGMA could not be read correctly
[runnervm76f27:05682] *** Process received signal ***
[runnervm76f27:05682] Signal: Aborted (6)
[runnervm76f27:05682] Signal code:  (-6)
[runnervm76f27:05682] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6325e45330]
[runnervm76f27:05682] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f6325e9ec0c]
[runnervm76f27:05682] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f6325e4527e]
[runnervm76f27:05682] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f6325e288ff]
[runnervm76f27:05682] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f63262a5ff5]
[runnervm76f27:05682] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f63262bb0da]
[runnervm76f27:05682] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f63262a5a55]
[runnervm76f27:05682] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f63262a5a6f]
[runnervm76f27:05682] [ 8] plumed(+0x146dd)[0x55f05bf236dd]
[runnervm76f27:05682] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f6325e2a1ca]
[runnervm76f27:05682] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f6325e2a28b]
[runnervm76f27:05682] [11] plumed(+0x15365)[0x55f05bf24365]
[runnervm76f27:05682] *** End of error message ***
</pre>
{% endraw %}

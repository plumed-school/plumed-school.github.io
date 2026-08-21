Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[runnervm76f27:05317] *** Process received signal ***
[runnervm76f27:05317] Signal: Aborted (6)
[runnervm76f27:05317] Signal code:  (-6)
[runnervm76f27:05317] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2dad245330]
[runnervm76f27:05317] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f2dad29ec0c]
[runnervm76f27:05317] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f2dad24527e]
[runnervm76f27:05317] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f2dad2288ff]
[runnervm76f27:05317] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2dad6a5ff5]
[runnervm76f27:05317] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2dad6bb0da]
[runnervm76f27:05317] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2dad6a5a55]
[runnervm76f27:05317] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2dad6a5a6f]
[runnervm76f27:05317] [ 8] plumed(+0x146dd)[0x559276a3a6dd]
[runnervm76f27:05317] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f2dad22a1ca]
[runnervm76f27:05317] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f2dad22a28b]
[runnervm76f27:05317] [11] plumed(+0x15365)[0x559276a3b365]
[runnervm76f27:05317] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  examples.md_working_4.dat   
Download: [zipped raw stdout](examples.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](examples.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action LOAD with label @0 : cannot understand the following words from the input line : GLOBAL
[runnervm76f27:04770] *** Process received signal ***
[runnervm76f27:04770] Signal: Aborted (6)
[runnervm76f27:04770] Signal code:  (-6)
[runnervm76f27:04770] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f77c6445330]
[runnervm76f27:04770] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f77c649ec0c]
[runnervm76f27:04770] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f77c644527e]
[runnervm76f27:04770] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f77c64288ff]
[runnervm76f27:04770] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f77c68a5ff5]
[runnervm76f27:04770] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f77c68bb0da]
[runnervm76f27:04770] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f77c68a5a55]
[runnervm76f27:04770] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f77c68a5a6f]
[runnervm76f27:04770] [ 8] plumed(+0x146dd)[0x5597452466dd]
[runnervm76f27:04770] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f77c642a1ca]
[runnervm76f27:04770] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f77c642a28b]
[runnervm76f27:04770] [11] plumed(+0x15365)[0x559745247365]
[runnervm76f27:04770] *** End of error message ***
</pre>
{% endraw %}

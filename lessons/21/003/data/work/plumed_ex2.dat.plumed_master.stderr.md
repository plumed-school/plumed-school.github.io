Stderr for source:  work/plumed_ex2.dat   
Download: [zipped raw stdout](plumed_ex2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @27 : keyword ARG is compulsory for this action
[runnervm76f27:05851] *** Process received signal ***
[runnervm76f27:05851] Signal: Aborted (6)
[runnervm76f27:05851] Signal code:  (-6)
[runnervm76f27:05851] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe422445330]
[runnervm76f27:05851] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe42249ec0c]
[runnervm76f27:05851] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe42244527e]
[runnervm76f27:05851] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe4224288ff]
[runnervm76f27:05851] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe4228a5ff5]
[runnervm76f27:05851] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe4228bb0da]
[runnervm76f27:05851] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe4228a5a55]
[runnervm76f27:05851] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe4228a5a6f]
[runnervm76f27:05851] [ 8] plumed_master(+0x146dd)[0x558b1aa1f6dd]
[runnervm76f27:05851] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe42242a1ca]
[runnervm76f27:05851] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe42242a28b]
[runnervm76f27:05851] [11] plumed_master(+0x15365)[0x558b1aa20365]
[runnervm76f27:05851] *** End of error message ***
</pre>
{% endraw %}

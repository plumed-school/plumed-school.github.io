Stderr for source:  INSTRUCTIONS.md_working_3.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[runnervm76f27:05361] *** Process received signal ***
[runnervm76f27:05361] Signal: Aborted (6)
[runnervm76f27:05361] Signal code:  (-6)
[runnervm76f27:05361] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4439845330]
[runnervm76f27:05361] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f443989ec0c]
[runnervm76f27:05361] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f443984527e]
[runnervm76f27:05361] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f44398288ff]
[runnervm76f27:05361] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4439ca5ff5]
[runnervm76f27:05361] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4439cbb0da]
[runnervm76f27:05361] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4439ca5a55]
[runnervm76f27:05361] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4439ca5a6f]
[runnervm76f27:05361] [ 8] plumed(+0x146dd)[0x558b1fa536dd]
[runnervm76f27:05361] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f443982a1ca]
[runnervm76f27:05361] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f443982a28b]
[runnervm76f27:05361] [11] plumed(+0x15365)[0x558b1fa54365]
[runnervm76f27:05361] *** End of error message ***
</pre>
{% endraw %}

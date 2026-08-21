Stderr for source:  examples.md_working_3.dat   
Download: [zipped raw stdout](examples.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](examples.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action LOAD with label @0 : cannot understand the following words from the input line : GLOBAL
[runnervm76f27:04725] *** Process received signal ***
[runnervm76f27:04725] Signal: Aborted (6)
[runnervm76f27:04725] Signal code:  (-6)
[runnervm76f27:04725] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9998045330]
[runnervm76f27:04725] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f999809ec0c]
[runnervm76f27:04725] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f999804527e]
[runnervm76f27:04725] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f99980288ff]
[runnervm76f27:04725] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f99984a5ff5]
[runnervm76f27:04725] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f99984bb0da]
[runnervm76f27:04725] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f99984a5a55]
[runnervm76f27:04725] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f99984a5a6f]
[runnervm76f27:04725] [ 8] plumed(+0x146dd)[0x56254d8916dd]
[runnervm76f27:04725] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f999802a1ca]
[runnervm76f27:04725] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f999802a28b]
[runnervm76f27:04725] [11] plumed(+0x15365)[0x56254d892365]
[runnervm76f27:04725] *** End of error message ***
</pre>
{% endraw %}

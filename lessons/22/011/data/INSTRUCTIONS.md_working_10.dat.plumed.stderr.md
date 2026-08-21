Stderr for source:  INSTRUCTIONS.md_working_10.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_10.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_10.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label dist : could not find file named colvar_reweight.data
[runnervm76f27:05554] *** Process received signal ***
[runnervm76f27:05554] Signal: Aborted (6)
[runnervm76f27:05554] Signal code:  (-6)
[runnervm76f27:05554] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9a0d645330]
[runnervm76f27:05554] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9a0d69ec0c]
[runnervm76f27:05554] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9a0d64527e]
[runnervm76f27:05554] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9a0d6288ff]
[runnervm76f27:05554] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9a0daa5ff5]
[runnervm76f27:05554] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9a0dabb0da]
[runnervm76f27:05554] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9a0daa5a55]
[runnervm76f27:05554] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9a0daa5a6f]
[runnervm76f27:05554] [ 8] plumed(+0x146dd)[0x55efc62f26dd]
[runnervm76f27:05554] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9a0d62a1ca]
[runnervm76f27:05554] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9a0d62a28b]
[runnervm76f27:05554] [11] plumed(+0x15365)[0x55efc62f3365]
[runnervm76f27:05554] *** End of error message ***
</pre>
{% endraw %}

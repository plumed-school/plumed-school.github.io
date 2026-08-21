Stderr for source:  examples.md_working_3.dat   
Download: [zipped raw stdout](examples.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](examples.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action LOAD with label @0 : cannot understand the following words from the input line : GLOBAL
[runnervm76f27:04741] *** Process received signal ***
[runnervm76f27:04741] Signal: Aborted (6)
[runnervm76f27:04741] Signal code:  (-6)
[runnervm76f27:04741] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9f5ea45330]
[runnervm76f27:04741] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9f5ea9ec0c]
[runnervm76f27:04741] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9f5ea4527e]
[runnervm76f27:04741] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9f5ea288ff]
[runnervm76f27:04741] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9f5eea5ff5]
[runnervm76f27:04741] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9f5eebb0da]
[runnervm76f27:04741] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9f5eea5a55]
[runnervm76f27:04741] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9f5eea5a6f]
[runnervm76f27:04741] [ 8] plumed_master(+0x146dd)[0x556e694e56dd]
[runnervm76f27:04741] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9f5ea2a1ca]
[runnervm76f27:04741] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9f5ea2a28b]
[runnervm76f27:04741] [11] plumed_master(+0x15365)[0x556e694e6365]
[runnervm76f27:04741] *** End of error message ***
</pre>
{% endraw %}

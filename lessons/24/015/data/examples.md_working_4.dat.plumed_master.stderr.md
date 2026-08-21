Stderr for source:  examples.md_working_4.dat   
Download: [zipped raw stdout](examples.md_working_4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](examples.md_working_4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action LOAD with label @0 : cannot understand the following words from the input line : GLOBAL
[runnervm76f27:04786] *** Process received signal ***
[runnervm76f27:04786] Signal: Aborted (6)
[runnervm76f27:04786] Signal code:  (-6)
[runnervm76f27:04786] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0444645330]
[runnervm76f27:04786] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f044469ec0c]
[runnervm76f27:04786] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f044464527e]
[runnervm76f27:04786] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f04446288ff]
[runnervm76f27:04786] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f0444aa5ff5]
[runnervm76f27:04786] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f0444abb0da]
[runnervm76f27:04786] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f0444aa5a55]
[runnervm76f27:04786] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f0444aa5a6f]
[runnervm76f27:04786] [ 8] plumed_master(+0x146dd)[0x556decf8f6dd]
[runnervm76f27:04786] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f044462a1ca]
[runnervm76f27:04786] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f044462a28b]
[runnervm76f27:04786] [11] plumed_master(+0x15365)[0x556decf90365]
[runnervm76f27:04786] *** End of error message ***
</pre>
{% endraw %}

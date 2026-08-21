Stderr for source:  INSTRUCTIONS.md_working_3.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label m : Calculating the transition bias on the fly works only with a grid
[runnervm76f27:05377] *** Process received signal ***
[runnervm76f27:05377] Signal: Aborted (6)
[runnervm76f27:05377] Signal code:  (-6)
[runnervm76f27:05377] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fe366a45330]
[runnervm76f27:05377] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fe366a9ec0c]
[runnervm76f27:05377] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fe366a4527e]
[runnervm76f27:05377] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fe366a288ff]
[runnervm76f27:05377] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fe366ea5ff5]
[runnervm76f27:05377] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fe366ebb0da]
[runnervm76f27:05377] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fe366ea5a55]
[runnervm76f27:05377] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fe366ea5a6f]
[runnervm76f27:05377] [ 8] plumed_master(+0x146dd)[0x55a3769326dd]
[runnervm76f27:05377] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fe366a2a1ca]
[runnervm76f27:05377] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fe366a2a28b]
[runnervm76f27:05377] [11] plumed_master(+0x15365)[0x55a376933365]
[runnervm76f27:05377] *** End of error message ***
</pre>
{% endraw %}

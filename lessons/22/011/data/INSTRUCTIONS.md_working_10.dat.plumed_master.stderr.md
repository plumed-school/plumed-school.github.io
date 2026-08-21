Stderr for source:  INSTRUCTIONS.md_working_10.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_10.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_10.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action READ with label dist : could not find file named colvar_reweight.data
[runnervm76f27:05569] *** Process received signal ***
[runnervm76f27:05569] Signal: Aborted (6)
[runnervm76f27:05569] Signal code:  (-6)
[runnervm76f27:05569] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f556fa45330]
[runnervm76f27:05569] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f556fa9ec0c]
[runnervm76f27:05569] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f556fa4527e]
[runnervm76f27:05569] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f556fa288ff]
[runnervm76f27:05569] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f556fea5ff5]
[runnervm76f27:05569] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f556febb0da]
[runnervm76f27:05569] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f556fea5a55]
[runnervm76f27:05569] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f556fea5a6f]
[runnervm76f27:05569] [ 8] plumed_master(+0x146dd)[0x5571e853b6dd]
[runnervm76f27:05569] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f556fa2a1ca]
[runnervm76f27:05569] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f556fa2a28b]
[runnervm76f27:05569] [11] plumed_master(+0x15365)[0x5571e853c365]
[runnervm76f27:05569] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  ./solutions/walker-0/plumed_reweight_newcv.dat   
Download: [zipped raw stdout](plumed_reweight_newcv.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight_newcv.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action DUMPGRID with label @23 : keyword ARG is compulsory for this action
[runnervm76f27:04098] *** Process received signal ***
[runnervm76f27:04098] Signal: Aborted (6)
[runnervm76f27:04098] Signal code:  (-6)
[runnervm76f27:04098] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f1097a45330]
[runnervm76f27:04098] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f1097a9ec0c]
[runnervm76f27:04098] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f1097a4527e]
[runnervm76f27:04098] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f1097a288ff]
[runnervm76f27:04098] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f1097ea5ff5]
[runnervm76f27:04098] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f1097ebb0da]
[runnervm76f27:04098] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f1097ea5a55]
[runnervm76f27:04098] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f1097ea5a6f]
[runnervm76f27:04098] [ 8] plumed_master(+0x146dd)[0x558d95aba6dd]
[runnervm76f27:04098] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f1097a2a1ca]
[runnervm76f27:04098] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f1097a2a28b]
[runnervm76f27:04098] [11] plumed_master(+0x15365)[0x558d95abb365]
[runnervm76f27:04098] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex2.dat   
Download: [zipped raw stdout](plumed_ex2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s80 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm76f27:05836] *** Process received signal ***
[runnervm76f27:05836] Signal: Aborted (6)
[runnervm76f27:05836] Signal code:  (-6)
[runnervm76f27:05836] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7ffb68c45330]
[runnervm76f27:05836] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7ffb68c9ec0c]
[runnervm76f27:05836] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7ffb68c4527e]
[runnervm76f27:05836] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7ffb68c288ff]
[runnervm76f27:05836] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7ffb690a5ff5]
[runnervm76f27:05836] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7ffb690bb0da]
[runnervm76f27:05836] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7ffb690a5a55]
[runnervm76f27:05836] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7ffb690a5a6f]
[runnervm76f27:05836] [ 8] plumed(+0x146dd)[0x5572e4ca36dd]
[runnervm76f27:05836] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7ffb68c2a1ca]
[runnervm76f27:05836] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7ffb68c2a28b]
[runnervm76f27:05836] [11] plumed(+0x15365)[0x5572e4ca4365]
[runnervm76f27:05836] *** End of error message ***
</pre>
{% endraw %}

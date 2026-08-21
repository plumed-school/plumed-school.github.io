Stderr for source:  work/plumed_ex4.dat   
Download: [zipped raw stdout](plumed_ex4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s16 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm76f27:06433] *** Process received signal ***
[runnervm76f27:06433] Signal: Aborted (6)
[runnervm76f27:06433] Signal code:  (-6)
[runnervm76f27:06433] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f5267c45330]
[runnervm76f27:06433] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f5267c9ec0c]
[runnervm76f27:06433] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f5267c4527e]
[runnervm76f27:06433] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f5267c288ff]
[runnervm76f27:06433] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f52680a5ff5]
[runnervm76f27:06433] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f52680bb0da]
[runnervm76f27:06433] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f52680a5a55]
[runnervm76f27:06433] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f52680a5a6f]
[runnervm76f27:06433] [ 8] plumed(+0x146dd)[0x5581aff526dd]
[runnervm76f27:06433] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f5267c2a1ca]
[runnervm76f27:06433] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f5267c2a28b]
[runnervm76f27:06433] [11] plumed(+0x15365)[0x5581aff53365]
[runnervm76f27:06433] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex4.dat   
Download: [zipped raw stdout](plumed_ex4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s16 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm76f27:06450] *** Process received signal ***
[runnervm76f27:06450] Signal: Aborted (6)
[runnervm76f27:06450] Signal code:  (-6)
[runnervm76f27:06450] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f42baa45330]
[runnervm76f27:06450] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f42baa9ec0c]
[runnervm76f27:06450] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f42baa4527e]
[runnervm76f27:06450] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f42baa288ff]
[runnervm76f27:06450] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f42baea5ff5]
[runnervm76f27:06450] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f42baebb0da]
[runnervm76f27:06450] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f42baea5a55]
[runnervm76f27:06450] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f42baea5a6f]
[runnervm76f27:06450] [ 8] plumed_master(+0x146dd)[0x55c35fe546dd]
[runnervm76f27:06450] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f42baa2a1ca]
[runnervm76f27:06450] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f42baa2a28b]
[runnervm76f27:06450] [11] plumed_master(+0x15365)[0x55c35fe55365]
[runnervm76f27:06450] *** End of error message ***
</pre>
{% endraw %}

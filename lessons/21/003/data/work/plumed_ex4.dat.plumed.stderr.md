Stderr for source:  work/plumed_ex4.dat   
Download: [zipped raw stdout](plumed_ex4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s74 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm76f27:05899] *** Process received signal ***
[runnervm76f27:05899] Signal: Aborted (6)
[runnervm76f27:05899] Signal code:  (-6)
[runnervm76f27:05899] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4bc0a45330]
[runnervm76f27:05899] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4bc0a9ec0c]
[runnervm76f27:05899] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4bc0a4527e]
[runnervm76f27:05899] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4bc0a288ff]
[runnervm76f27:05899] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4bc0ea5ff5]
[runnervm76f27:05899] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4bc0ebb0da]
[runnervm76f27:05899] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4bc0ea5a55]
[runnervm76f27:05899] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4bc0ea5a6f]
[runnervm76f27:05899] [ 8] plumed(+0x146dd)[0x564408eab6dd]
[runnervm76f27:05899] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4bc0a2a1ca]
[runnervm76f27:05899] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4bc0a2a28b]
[runnervm76f27:05899] [11] plumed(+0x15365)[0x564408eac365]
[runnervm76f27:05899] *** End of error message ***
</pre>
{% endraw %}

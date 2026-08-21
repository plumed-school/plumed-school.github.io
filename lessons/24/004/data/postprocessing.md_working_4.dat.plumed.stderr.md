Stderr for source:  postprocessing.md_working_4.dat   
Download: [zipped raw stdout](postprocessing.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](postprocessing.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HISTOGRAM with label @s14 : set NORMALIZATION=true/false when using LOGWEIGHTS as otherwise the weights are ignored. Alternatively, learn to use the new syntax for histograms with KDE/ACCUMULATE to have more control over what PLUMED is calculating
[runnervm76f27:05351] *** Process received signal ***
[runnervm76f27:05351] Signal: Aborted (6)
[runnervm76f27:05351] Signal code:  (-6)
[runnervm76f27:05351] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9f2fe45330]
[runnervm76f27:05351] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9f2fe9ec0c]
[runnervm76f27:05351] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9f2fe4527e]
[runnervm76f27:05351] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9f2fe288ff]
[runnervm76f27:05351] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9f302a5ff5]
[runnervm76f27:05351] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9f302bb0da]
[runnervm76f27:05351] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9f302a5a55]
[runnervm76f27:05351] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9f302a5a6f]
[runnervm76f27:05351] [ 8] plumed(+0x146dd)[0x55b042f126dd]
[runnervm76f27:05351] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9f2fe2a1ca]
[runnervm76f27:05351] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9f2fe2a28b]
[runnervm76f27:05351] [11] plumed(+0x15365)[0x55b042f13365]
[runnervm76f27:05351] *** End of error message ***
</pre>
{% endraw %}

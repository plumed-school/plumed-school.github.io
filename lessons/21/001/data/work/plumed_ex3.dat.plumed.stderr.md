Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():

(core/GenericMolInfo.cpp:324) void PLMD::GenericMolInfo::interpretSymbol(const std::string&, std::vector<PLMD::AtomNumber>&)
Error importing MDAnalysis module: No module named 'MDAnalysis'
[runnervm76f27:06562] *** Process received signal ***
[runnervm76f27:06562] Signal: Aborted (6)
[runnervm76f27:06562] Signal code:  (-6)
[runnervm76f27:06562] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa85a445330]
[runnervm76f27:06562] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa85a49ec0c]
[runnervm76f27:06562] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa85a44527e]
[runnervm76f27:06562] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa85a4288ff]
[runnervm76f27:06562] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa85a8a5ff5]
[runnervm76f27:06562] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa85a8bb0da]
[runnervm76f27:06562] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa85a8a5a55]
[runnervm76f27:06562] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa85a8a5a6f]
[runnervm76f27:06562] [ 8] plumed(+0x146dd)[0x56459ffcd6dd]
[runnervm76f27:06562] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa85a42a1ca]
[runnervm76f27:06562] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa85a42a28b]
[runnervm76f27:06562] [11] plumed(+0x15365)[0x56459ffce365]
[runnervm76f27:06562] *** End of error message ***
</pre>
{% endraw %}

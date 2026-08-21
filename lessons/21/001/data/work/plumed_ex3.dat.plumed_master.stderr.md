Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():

(core/GenericMolInfo.cpp:324) void PLMD::GenericMolInfo::interpretSymbol(const std::string&, std::vector<PLMD::AtomNumber>&)
Error importing MDAnalysis module: No module named 'MDAnalysis'
[runnervm76f27:06584] *** Process received signal ***
[runnervm76f27:06584] Signal: Aborted (6)
[runnervm76f27:06584] Signal code:  (-6)
[runnervm76f27:06584] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fc564c45330]
[runnervm76f27:06584] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fc564c9ec0c]
[runnervm76f27:06584] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fc564c4527e]
[runnervm76f27:06584] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fc564c288ff]
[runnervm76f27:06584] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fc5650a5ff5]
[runnervm76f27:06584] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fc5650bb0da]
[runnervm76f27:06584] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fc5650a5a55]
[runnervm76f27:06584] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fc5650a5a6f]
[runnervm76f27:06584] [ 8] plumed_master(+0x146dd)[0x5605d06c96dd]
[runnervm76f27:06584] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fc564c2a1ca]
[runnervm76f27:06584] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fc564c2a28b]
[runnervm76f27:06584] [11] plumed_master(+0x15365)[0x5605d06ca365]
[runnervm76f27:06584] *** End of error message ***
</pre>
{% endraw %}

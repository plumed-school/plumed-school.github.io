Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():

(core/GenericMolInfo.cpp:324) void PLMD::GenericMolInfo::interpretSymbol(const std::string&, std::vector<PLMD::AtomNumber>&)
Error importing MDAnalysis module: No module named 'MDAnalysis'
[runnervm76f27:06638] *** Process received signal ***
[runnervm76f27:06638] Signal: Aborted (6)
[runnervm76f27:06638] Signal code:  (-6)
[runnervm76f27:06638] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7feabae45330]
[runnervm76f27:06638] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7feabae9ec0c]
[runnervm76f27:06638] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7feabae4527e]
[runnervm76f27:06638] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7feabae288ff]
[runnervm76f27:06638] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7feabb2a5ff5]
[runnervm76f27:06638] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7feabb2bb0da]
[runnervm76f27:06638] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7feabb2a5a55]
[runnervm76f27:06638] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7feabb2a5a6f]
[runnervm76f27:06638] [ 8] plumed(+0x146dd)[0x5617bea296dd]
[runnervm76f27:06638] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7feabae2a1ca]
[runnervm76f27:06638] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7feabae2a28b]
[runnervm76f27:06638] [11] plumed(+0x15365)[0x5617bea2a365]
[runnervm76f27:06638] *** End of error message ***
</pre>
{% endraw %}

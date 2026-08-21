Stderr for source:  GAT_SAFE_README.md_working_1.dat   
Download: [zipped raw stdout](GAT_SAFE_README.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](GAT_SAFE_README.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file input.ala2.pdb
[runnervm76f27:04209] *** Process received signal ***
[runnervm76f27:04209] Signal: Aborted (6)
[runnervm76f27:04209] Signal code:  (-6)
[runnervm76f27:04209] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f0609445330]
[runnervm76f27:04209] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f060949ec0c]
[runnervm76f27:04209] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f060944527e]
[runnervm76f27:04209] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f06094288ff]
[runnervm76f27:04209] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f06098a5ff5]
[runnervm76f27:04209] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f06098bb0da]
[runnervm76f27:04209] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f06098a5a55]
[runnervm76f27:04209] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f06098a5a6f]
[runnervm76f27:04209] [ 8] plumed(+0x146dd)[0x55bce4e726dd]
[runnervm76f27:04209] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f060942a1ca]
[runnervm76f27:04209] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f060942a28b]
[runnervm76f27:04209] [11] plumed(+0x15365)[0x55bce4e73365]
[runnervm76f27:04209] *** End of error message ***
</pre>
{% endraw %}

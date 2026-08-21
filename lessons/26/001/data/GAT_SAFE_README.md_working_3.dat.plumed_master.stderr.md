Stderr for source:  GAT_SAFE_README.md_working_3.dat   
Download: [zipped raw stdout](GAT_SAFE_README.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](GAT_SAFE_README.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file input.ala2.pdb
[runnervm76f27:04313] *** Process received signal ***
[runnervm76f27:04313] Signal: Aborted (6)
[runnervm76f27:04313] Signal code:  (-6)
[runnervm76f27:04313] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f2951645330]
[runnervm76f27:04313] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f295169ec0c]
[runnervm76f27:04313] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f295164527e]
[runnervm76f27:04313] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f29516288ff]
[runnervm76f27:04313] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f2951aa5ff5]
[runnervm76f27:04313] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f2951abb0da]
[runnervm76f27:04313] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f2951aa5a55]
[runnervm76f27:04313] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f2951aa5a6f]
[runnervm76f27:04313] [ 8] plumed_master(+0x146dd)[0x55af99d276dd]
[runnervm76f27:04313] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f295162a1ca]
[runnervm76f27:04313] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f295162a28b]
[runnervm76f27:04313] [11] plumed_master(+0x15365)[0x55af99d28365]
[runnervm76f27:04313] *** End of error message ***
</pre>
{% endraw %}

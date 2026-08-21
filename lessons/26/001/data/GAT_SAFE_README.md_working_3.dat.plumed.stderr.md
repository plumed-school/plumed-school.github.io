Stderr for source:  GAT_SAFE_README.md_working_3.dat   
Download: [zipped raw stdout](GAT_SAFE_README.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](GAT_SAFE_README.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:93) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file input.ala2.pdb
[runnervm76f27:04297] *** Process received signal ***
[runnervm76f27:04297] Signal: Aborted (6)
[runnervm76f27:04297] Signal code:  (-6)
[runnervm76f27:04297] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f385ec45330]
[runnervm76f27:04297] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f385ec9ec0c]
[runnervm76f27:04297] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f385ec4527e]
[runnervm76f27:04297] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f385ec288ff]
[runnervm76f27:04297] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f385f0a5ff5]
[runnervm76f27:04297] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f385f0bb0da]
[runnervm76f27:04297] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f385f0a5a55]
[runnervm76f27:04297] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f385f0a5a6f]
[runnervm76f27:04297] [ 8] plumed(+0x146dd)[0x55be80d696dd]
[runnervm76f27:04297] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f385ec2a1ca]
[runnervm76f27:04297] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f385ec2a28b]
[runnervm76f27:04297] [11] plumed(+0x15365)[0x55be80d6a365]
[runnervm76f27:04297] *** End of error message ***
</pre>
{% endraw %}

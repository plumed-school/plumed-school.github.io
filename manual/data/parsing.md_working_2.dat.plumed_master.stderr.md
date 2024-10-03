Stderr for source:  manual/data/parsing.md_working_2.dat   
Download: [zipped raw stdout](parsing.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](parsing.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/GenericMolInfo.cpp:89) PLMD::GenericMolInfo::GenericMolInfo(const PLMD::ActionOptions&)
missing input file AA.pdb
[fv-az740-873:41019] *** Process received signal ***
[fv-az740-873:41019] Signal: Aborted (6)
[fv-az740-873:41019] Signal code:  (-6)
[fv-az740-873:41019] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbcbc842520]
[fv-az740-873:41019] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbcbc8969fc]
[fv-az740-873:41019] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbcbc842476]
[fv-az740-873:41019] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbcbc8287f3]
[fv-az740-873:41019] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbcbcca2b9e]
[fv-az740-873:41019] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbcbccae20c]
[fv-az740-873:41019] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbcbccae277]
[fv-az740-873:41019] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbcbccae52b]
[fv-az740-873:41019] [ 8] plumed_master(+0x14274)[0x560f0846a274]
[fv-az740-873:41019] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbcbc829d90]
[fv-az740-873:41019] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbcbc829e40]
[fv-az740-873:41019] [11] plumed_master(+0x14ed5)[0x560f0846aed5]
[fv-az740-873:41019] *** End of error message ***
</pre>
{% endraw %}

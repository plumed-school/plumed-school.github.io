Stderr for source:  RMSD.md_working_1.dat   
Download: [zipped raw stdout](RMSD.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONSTANT with label v : cannot understand the following words from the input line : NCOLS=12, NROWS=2
[fv-az714-382:08299] *** Process received signal ***
[fv-az714-382:08299] Signal: Aborted (6)
[fv-az714-382:08299] Signal code:  (-6)
[fv-az714-382:08299] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fad17242520]
[fv-az714-382:08299] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fad172969fc]
[fv-az714-382:08299] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fad17242476]
[fv-az714-382:08299] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fad172287f3]
[fv-az714-382:08299] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fad176a2b9e]
[fv-az714-382:08299] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fad176ae20c]
[fv-az714-382:08299] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fad176ae277]
[fv-az714-382:08299] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fad176ae52b]
[fv-az714-382:08299] [ 8] plumed(+0x12f48)[0x563ad107cf48]
[fv-az714-382:08299] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fad17229d90]
[fv-az714-382:08299] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fad17229e40]
[fv-az714-382:08299] [11] plumed(+0x131e5)[0x563ad107d1e5]
[fv-az714-382:08299] *** End of error message ***
</pre>
{% endraw %}

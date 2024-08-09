Stderr for source:  RMSD.md_working_6.dat   
Download: [zipped raw stdout](RMSD.md_working_6.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_6.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action RMSD with label rmsd : cannot understand the following words from the input line : DISPLACEMENT
[fv-az714-382:08451] *** Process received signal ***
[fv-az714-382:08451] Signal: Aborted (6)
[fv-az714-382:08451] Signal code:  (-6)
[fv-az714-382:08451] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6467a42520]
[fv-az714-382:08451] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6467a969fc]
[fv-az714-382:08451] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6467a42476]
[fv-az714-382:08451] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6467a287f3]
[fv-az714-382:08451] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6467ea2b9e]
[fv-az714-382:08451] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6467eae20c]
[fv-az714-382:08451] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6467eae277]
[fv-az714-382:08451] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6467eae52b]
[fv-az714-382:08451] [ 8] plumed(+0x12f48)[0x562f929dcf48]
[fv-az714-382:08451] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6467a29d90]
[fv-az714-382:08451] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6467a29e40]
[fv-az714-382:08451] [11] plumed(+0x131e5)[0x562f929dd1e5]
[fv-az714-382:08451] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex1.dat   
Download: [zipped raw stdout](plumed_ex1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: DUMPPDB ATOMS=cc_data ATOM_INDICES=@nonhydrogens FILE=traj.pdb
Maybe a missing space or a typo?
[fv-az714-382:09008] *** Process received signal ***
[fv-az714-382:09008] Signal: Aborted (6)
[fv-az714-382:09008] Signal code:  (-6)
[fv-az714-382:09008] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fcf2e042520]
[fv-az714-382:09008] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fcf2e0969fc]
[fv-az714-382:09008] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fcf2e042476]
[fv-az714-382:09008] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fcf2e0287f3]
[fv-az714-382:09008] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fcf2e4a2b9e]
[fv-az714-382:09008] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fcf2e4ae20c]
[fv-az714-382:09008] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fcf2e4ae277]
[fv-az714-382:09008] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fcf2e4ae52b]
[fv-az714-382:09008] [ 8] plumed(+0x12f48)[0x5592010e3f48]
[fv-az714-382:09008] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fcf2e029d90]
[fv-az714-382:09008] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fcf2e029e40]
[fv-az714-382:09008] [11] plumed(+0x131e5)[0x5592010e41e5]
[fv-az714-382:09008] *** End of error message ***
</pre>
{% endraw %}

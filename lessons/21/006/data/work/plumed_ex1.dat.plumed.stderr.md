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
[fv-az1106-805:42973] *** Process received signal ***
[fv-az1106-805:42973] Signal: Aborted (6)
[fv-az1106-805:42973] Signal code:  (-6)
[fv-az1106-805:42973] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f137ac42520]
[fv-az1106-805:42973] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f137ac969fc]
[fv-az1106-805:42973] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f137ac42476]
[fv-az1106-805:42973] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f137ac287f3]
[fv-az1106-805:42973] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f137b0a2b9e]
[fv-az1106-805:42973] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f137b0ae20c]
[fv-az1106-805:42973] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f137b0ae277]
[fv-az1106-805:42973] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f137b0ae52b]
[fv-az1106-805:42973] [ 8] plumed(+0x12f48)[0x5649e521af48]
[fv-az1106-805:42973] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f137ac29d90]
[fv-az1106-805:42973] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f137ac29e40]
[fv-az1106-805:42973] [11] plumed(+0x131e5)[0x5649e521b1e5]
[fv-az1106-805:42973] *** End of error message ***
</pre>
{% endraw %}

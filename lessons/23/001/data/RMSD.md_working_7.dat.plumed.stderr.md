Stderr for source:  RMSD.md_working_7.dat   
Download: [zipped raw stdout](RMSD.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PDB2CONSTANT LABEL=rmsd_ref REFERENCE=reference.pdb
Maybe a missing space or a typo?
[fv-az1106-805:42442] *** Process received signal ***
[fv-az1106-805:42442] Signal: Aborted (6)
[fv-az1106-805:42442] Signal code:  (-6)
[fv-az1106-805:42442] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbbd4242520]
[fv-az1106-805:42442] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbbd42969fc]
[fv-az1106-805:42442] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbbd4242476]
[fv-az1106-805:42442] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbbd42287f3]
[fv-az1106-805:42442] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbbd46a2b9e]
[fv-az1106-805:42442] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbbd46ae20c]
[fv-az1106-805:42442] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbbd46ae277]
[fv-az1106-805:42442] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbbd46ae52b]
[fv-az1106-805:42442] [ 8] plumed(+0x12f48)[0x55a42424cf48]
[fv-az1106-805:42442] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbbd4229d90]
[fv-az1106-805:42442] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbbd4229e40]
[fv-az1106-805:42442] [11] plumed(+0x131e5)[0x55a42424d1e5]
[fv-az1106-805:42442] *** End of error message ***
</pre>
{% endraw %}

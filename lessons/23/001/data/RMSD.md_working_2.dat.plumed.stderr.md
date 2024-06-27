Stderr for source:  RMSD.md_working_2.dat   
Download: [zipped raw stdout](RMSD.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: DISPLACEMENT LABEL=disp ARG1=d1,d2,d3 ARG2=d1_ref,d2_ref,d3_ref
Maybe a missing space or a typo?
[fv-az1106-805:42292] *** Process received signal ***
[fv-az1106-805:42292] Signal: Aborted (6)
[fv-az1106-805:42292] Signal code:  (-6)
[fv-az1106-805:42292] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f88e9642520]
[fv-az1106-805:42292] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f88e96969fc]
[fv-az1106-805:42292] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f88e9642476]
[fv-az1106-805:42292] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f88e96287f3]
[fv-az1106-805:42292] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f88e9aa2b9e]
[fv-az1106-805:42292] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f88e9aae20c]
[fv-az1106-805:42292] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f88e9aae277]
[fv-az1106-805:42292] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f88e9aae52b]
[fv-az1106-805:42292] [ 8] plumed(+0x12f48)[0x55f97418af48]
[fv-az1106-805:42292] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f88e9629d90]
[fv-az1106-805:42292] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f88e9629e40]
[fv-az1106-805:42292] [11] plumed(+0x131e5)[0x55f97418b1e5]
[fv-az1106-805:42292] *** End of error message ***
</pre>
{% endraw %}

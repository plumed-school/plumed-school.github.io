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
[fv-az659-187:41994] *** Process received signal ***
[fv-az659-187:41994] Signal: Aborted (6)
[fv-az659-187:41994] Signal code:  (-6)
[fv-az659-187:41994] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa68b642520]
[fv-az659-187:41994] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa68b6969fc]
[fv-az659-187:41994] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa68b642476]
[fv-az659-187:41994] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa68b6287f3]
[fv-az659-187:41994] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa68baa2b9e]
[fv-az659-187:41994] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa68baae20c]
[fv-az659-187:41994] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa68baae277]
[fv-az659-187:41994] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa68baae52b]
[fv-az659-187:41994] [ 8] plumed(+0x12f48)[0x55e29aa05f48]
[fv-az659-187:41994] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa68b629d90]
[fv-az659-187:41994] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa68b629e40]
[fv-az659-187:41994] [11] plumed(+0x131e5)[0x55e29aa061e5]
[fv-az659-187:41994] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex4.dat   
Download: [zipped raw stdout](plumed_ex4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex4.dat.plumed.stderr.txt.zip) 
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
[fv-az659-187:42085] *** Process received signal ***
[fv-az659-187:42085] Signal: Aborted (6)
[fv-az659-187:42085] Signal code:  (-6)
[fv-az659-187:42085] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc94ee42520]
[fv-az659-187:42085] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc94ee969fc]
[fv-az659-187:42085] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc94ee42476]
[fv-az659-187:42085] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc94ee287f3]
[fv-az659-187:42085] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc94f2a2b9e]
[fv-az659-187:42085] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc94f2ae20c]
[fv-az659-187:42085] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc94f2ae277]
[fv-az659-187:42085] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc94f2ae52b]
[fv-az659-187:42085] [ 8] plumed(+0x12f48)[0x563d02392f48]
[fv-az659-187:42085] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc94ee29d90]
[fv-az659-187:42085] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc94ee29e40]
[fv-az659-187:42085] [11] plumed(+0x131e5)[0x563d023931e5]
[fv-az659-187:42085] *** End of error message ***
</pre>
{% endraw %}

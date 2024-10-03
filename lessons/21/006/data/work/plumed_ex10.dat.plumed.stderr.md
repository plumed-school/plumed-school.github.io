Stderr for source:  work/plumed_ex10.dat   
Download: [zipped raw stdout](plumed_ex10.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex10.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: MORE_THAN LABEL=fcub ARG=cub SWITCH=SMAP R_0=0.45 D_0=0.0 A=8 B=8
Maybe a missing space or a typo?
[fv-az659-187:42265] *** Process received signal ***
[fv-az659-187:42265] Signal: Aborted (6)
[fv-az659-187:42265] Signal code:  (-6)
[fv-az659-187:42265] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1779042520]
[fv-az659-187:42265] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f17790969fc]
[fv-az659-187:42265] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1779042476]
[fv-az659-187:42265] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f17790287f3]
[fv-az659-187:42265] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f17794a2b9e]
[fv-az659-187:42265] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f17794ae20c]
[fv-az659-187:42265] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f17794ae277]
[fv-az659-187:42265] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f17794ae52b]
[fv-az659-187:42265] [ 8] plumed(+0x12f48)[0x562395706f48]
[fv-az659-187:42265] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1779029d90]
[fv-az659-187:42265] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1779029e40]
[fv-az659-187:42265] [11] plumed(+0x131e5)[0x5623957071e5]
[fv-az659-187:42265] *** End of error message ***
</pre>
{% endraw %}

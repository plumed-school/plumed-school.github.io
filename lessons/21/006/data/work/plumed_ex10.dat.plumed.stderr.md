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
[fv-az714-382:09281] *** Process received signal ***
[fv-az714-382:09281] Signal: Aborted (6)
[fv-az714-382:09281] Signal code:  (-6)
[fv-az714-382:09281] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f64eea42520]
[fv-az714-382:09281] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f64eea969fc]
[fv-az714-382:09281] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f64eea42476]
[fv-az714-382:09281] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f64eea287f3]
[fv-az714-382:09281] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f64eeea2b9e]
[fv-az714-382:09281] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f64eeeae20c]
[fv-az714-382:09281] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f64eeeae277]
[fv-az714-382:09281] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f64eeeae52b]
[fv-az714-382:09281] [ 8] plumed(+0x12f48)[0x5635a5025f48]
[fv-az714-382:09281] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f64eea29d90]
[fv-az714-382:09281] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f64eea29e40]
[fv-az714-382:09281] [11] plumed(+0x131e5)[0x5635a50261e5]
[fv-az714-382:09281] *** End of error message ***
</pre>
{% endraw %}

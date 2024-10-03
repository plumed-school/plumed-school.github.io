Stderr for source:  histograms.md_working_7.dat   
Download: [zipped raw stdout](histograms.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: PAIRENTROPY LABEL=pp GROUP=1-108 MAXR=2.0 GRID_BIN=20 CUTOFF=1.5 BANDWIDTH=0.13
Maybe a missing space or a typo?
[fv-az714-650:43783] *** Process received signal ***
[fv-az714-650:43783] Signal: Aborted (6)
[fv-az714-650:43783] Signal code:  (-6)
[fv-az714-650:43783] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f26fe042520]
[fv-az714-650:43783] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f26fe0969fc]
[fv-az714-650:43783] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f26fe042476]
[fv-az714-650:43783] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f26fe0287f3]
[fv-az714-650:43783] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f26fe4a2b9e]
[fv-az714-650:43783] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f26fe4ae20c]
[fv-az714-650:43783] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f26fe4ae277]
[fv-az714-650:43783] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f26fe4ae52b]
[fv-az714-650:43783] [ 8] plumed(+0x12f48)[0x55e10dde4f48]
[fv-az714-650:43783] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f26fe029d90]
[fv-az714-650:43783] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f26fe029e40]
[fv-az714-650:43783] [11] plumed(+0x131e5)[0x55e10dde51e5]
[fv-az714-650:43783] *** End of error message ***
</pre>
{% endraw %}

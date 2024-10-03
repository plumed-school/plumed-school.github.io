Stderr for source:  histograms.md_working_12.dat   
Download: [zipped raw stdout](histograms.md_working_12.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_12.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: KDE LABEL=hA_kde ARG=x GRID_MIN=0.0 GRID_MAX=3.0 GRID_BIN=100 BANDWIDTH=0.1 VOLUMES=f
Maybe a missing space or a typo?
[fv-az714-650:43943] *** Process received signal ***
[fv-az714-650:43943] Signal: Aborted (6)
[fv-az714-650:43943] Signal code:  (-6)
[fv-az714-650:43943] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb138042520]
[fv-az714-650:43943] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb1380969fc]
[fv-az714-650:43943] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb138042476]
[fv-az714-650:43943] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb1380287f3]
[fv-az714-650:43943] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb1384a2b9e]
[fv-az714-650:43943] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb1384ae20c]
[fv-az714-650:43943] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb1384ae277]
[fv-az714-650:43943] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb1384ae52b]
[fv-az714-650:43943] [ 8] plumed(+0x12f48)[0x556a442a7f48]
[fv-az714-650:43943] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb138029d90]
[fv-az714-650:43943] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb138029e40]
[fv-az714-650:43943] [11] plumed(+0x131e5)[0x556a442a81e5]
[fv-az714-650:43943] *** End of error message ***
</pre>
{% endraw %}

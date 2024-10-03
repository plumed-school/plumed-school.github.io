Stderr for source:  histograms.md_working_4.dat   
Download: [zipped raw stdout](histograms.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: KDE LABEL=hA_kde ARG=c1 GRID_MIN=0.0 GRID_MAX=12.0 GRID_BIN=120 BANDWIDTH=0.1
Maybe a missing space or a typo?
[fv-az714-650:43691] *** Process received signal ***
[fv-az714-650:43691] Signal: Aborted (6)
[fv-az714-650:43691] Signal code:  (-6)
[fv-az714-650:43691] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5740242520]
[fv-az714-650:43691] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f57402969fc]
[fv-az714-650:43691] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5740242476]
[fv-az714-650:43691] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f57402287f3]
[fv-az714-650:43691] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f57406a2b9e]
[fv-az714-650:43691] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f57406ae20c]
[fv-az714-650:43691] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f57406ae277]
[fv-az714-650:43691] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f57406ae52b]
[fv-az714-650:43691] [ 8] plumed(+0x12f48)[0x5628db26ef48]
[fv-az714-650:43691] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5740229d90]
[fv-az714-650:43691] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5740229e40]
[fv-az714-650:43691] [11] plumed(+0x131e5)[0x5628db26f1e5]
[fv-az714-650:43691] *** End of error message ***
</pre>
{% endraw %}

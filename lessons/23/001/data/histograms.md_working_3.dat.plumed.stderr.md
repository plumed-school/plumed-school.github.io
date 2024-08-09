Stderr for source:  histograms.md_working_3.dat   
Download: [zipped raw stdout](histograms.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: KDE LABEL=hA_kde ARG=x GRID_MIN=0.0 GRID_MAX=3.0 GRID_BIN=100 HEIGHTS=hA_h METRIC=hA_icov
Maybe a missing space or a typo?
[fv-az714-382:07860] *** Process received signal ***
[fv-az714-382:07860] Signal: Aborted (6)
[fv-az714-382:07860] Signal code:  (-6)
[fv-az714-382:07860] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0d91242520]
[fv-az714-382:07860] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0d912969fc]
[fv-az714-382:07860] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0d91242476]
[fv-az714-382:07860] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0d912287f3]
[fv-az714-382:07860] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0d916a2b9e]
[fv-az714-382:07860] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0d916ae20c]
[fv-az714-382:07860] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0d916ae277]
[fv-az714-382:07860] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0d916ae52b]
[fv-az714-382:07860] [ 8] plumed(+0x12f48)[0x55f1801d1f48]
[fv-az714-382:07860] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0d91229d90]
[fv-az714-382:07860] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0d91229e40]
[fv-az714-382:07860] [11] plumed(+0x131e5)[0x55f1801d21e5]
[fv-az714-382:07860] *** End of error message ***
</pre>
{% endraw %}

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
[fv-az1106-805:41946] *** Process received signal ***
[fv-az1106-805:41946] Signal: Aborted (6)
[fv-az1106-805:41946] Signal code:  (-6)
[fv-az1106-805:41946] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5b60642520]
[fv-az1106-805:41946] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5b606969fc]
[fv-az1106-805:41946] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5b60642476]
[fv-az1106-805:41946] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5b606287f3]
[fv-az1106-805:41946] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5b60aa2b9e]
[fv-az1106-805:41946] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5b60aae20c]
[fv-az1106-805:41946] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5b60aae277]
[fv-az1106-805:41946] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5b60aae52b]
[fv-az1106-805:41946] [ 8] plumed(+0x12f48)[0x558579c91f48]
[fv-az1106-805:41946] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5b60629d90]
[fv-az1106-805:41946] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5b60629e40]
[fv-az1106-805:41946] [11] plumed(+0x131e5)[0x558579c921e5]
[fv-az1106-805:41946] *** End of error message ***
</pre>
{% endraw %}

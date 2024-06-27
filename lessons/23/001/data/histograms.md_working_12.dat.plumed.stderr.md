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
[fv-az1106-805:42105] *** Process received signal ***
[fv-az1106-805:42105] Signal: Aborted (6)
[fv-az1106-805:42105] Signal code:  (-6)
[fv-az1106-805:42105] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fbcf2642520]
[fv-az1106-805:42105] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fbcf26969fc]
[fv-az1106-805:42105] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fbcf2642476]
[fv-az1106-805:42105] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fbcf26287f3]
[fv-az1106-805:42105] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fbcf2aa2b9e]
[fv-az1106-805:42105] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fbcf2aae20c]
[fv-az1106-805:42105] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fbcf2aae277]
[fv-az1106-805:42105] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fbcf2aae52b]
[fv-az1106-805:42105] [ 8] plumed(+0x12f48)[0x55598e1fdf48]
[fv-az1106-805:42105] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fbcf2629d90]
[fv-az1106-805:42105] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fbcf2629e40]
[fv-az1106-805:42105] [11] plumed(+0x131e5)[0x55598e1fe1e5]
[fv-az1106-805:42105] *** End of error message ***
</pre>
{% endraw %}

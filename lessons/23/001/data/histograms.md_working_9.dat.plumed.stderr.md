Stderr for source:  histograms.md_working_9.dat   
Download: [zipped raw stdout](histograms.md_working_9.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_9.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCES with label d1 : keyword ATOMS could not be read correctly
[fv-az714-650:43852] *** Process received signal ***
[fv-az714-650:43852] Signal: Aborted (6)
[fv-az714-650:43852] Signal code:  (-6)
[fv-az714-650:43852] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f63f4842520]
[fv-az714-650:43852] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f63f48969fc]
[fv-az714-650:43852] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f63f4842476]
[fv-az714-650:43852] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f63f48287f3]
[fv-az714-650:43852] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f63f4ca2b9e]
[fv-az714-650:43852] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f63f4cae20c]
[fv-az714-650:43852] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f63f4cae277]
[fv-az714-650:43852] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f63f4cae52b]
[fv-az714-650:43852] [ 8] plumed(+0x12f48)[0x55fbe65cff48]
[fv-az714-650:43852] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f63f4829d90]
[fv-az714-650:43852] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f63f4829e40]
[fv-az714-650:43852] [11] plumed(+0x131e5)[0x55fbe65d01e5]
[fv-az714-650:43852] *** End of error message ***
</pre>
{% endraw %}

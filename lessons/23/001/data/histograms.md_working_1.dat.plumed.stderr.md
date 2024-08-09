Stderr for source:  histograms.md_working_1.dat   
Download: [zipped raw stdout](histograms.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](histograms.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @2 : keyword GRID is compulsory for this action
[fv-az714-382:07799] *** Process received signal ***
[fv-az714-382:07799] Signal: Aborted (6)
[fv-az714-382:07799] Signal code:  (-6)
[fv-az714-382:07799] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8e94c42520]
[fv-az714-382:07799] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8e94c969fc]
[fv-az714-382:07799] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8e94c42476]
[fv-az714-382:07799] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8e94c287f3]
[fv-az714-382:07799] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8e950a2b9e]
[fv-az714-382:07799] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8e950ae20c]
[fv-az714-382:07799] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8e950ae277]
[fv-az714-382:07799] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8e950ae52b]
[fv-az714-382:07799] [ 8] plumed(+0x12f48)[0x55da9f667f48]
[fv-az714-382:07799] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8e94c29d90]
[fv-az714-382:07799] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8e94c29e40]
[fv-az714-382:07799] [11] plumed(+0x131e5)[0x55da9f6681e5]
[fv-az714-382:07799] *** End of error message ***
</pre>
{% endraw %}

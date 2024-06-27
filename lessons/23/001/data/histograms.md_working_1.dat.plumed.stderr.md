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
[fv-az1106-805:41765] *** Process received signal ***
[fv-az1106-805:41765] Signal: Aborted (6)
[fv-az1106-805:41765] Signal code:  (-6)
[fv-az1106-805:41765] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f68d0e42520]
[fv-az1106-805:41765] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f68d0e969fc]
[fv-az1106-805:41765] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f68d0e42476]
[fv-az1106-805:41765] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f68d0e287f3]
[fv-az1106-805:41765] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f68d12a2b9e]
[fv-az1106-805:41765] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f68d12ae20c]
[fv-az1106-805:41765] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f68d12ae277]
[fv-az1106-805:41765] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f68d12ae52b]
[fv-az1106-805:41765] [ 8] plumed(+0x12f48)[0x55f572cbef48]
[fv-az1106-805:41765] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f68d0e29d90]
[fv-az1106-805:41765] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f68d0e29e40]
[fv-az1106-805:41765] [11] plumed(+0x131e5)[0x55f572cbf1e5]
[fv-az1106-805:41765] *** End of error message ***
</pre>
{% endraw %}

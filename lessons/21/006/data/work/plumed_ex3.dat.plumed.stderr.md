Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action LANDMARK_SELECT_FPS with label fps : input analysis action was not specified use USE_OUTPUT_DATA_FROM
[fv-az714-382:09069] *** Process received signal ***
[fv-az714-382:09069] Signal: Aborted (6)
[fv-az714-382:09069] Signal code:  (-6)
[fv-az714-382:09069] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9a13e42520]
[fv-az714-382:09069] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9a13e969fc]
[fv-az714-382:09069] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9a13e42476]
[fv-az714-382:09069] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9a13e287f3]
[fv-az714-382:09069] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f9a142a2b9e]
[fv-az714-382:09069] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f9a142ae20c]
[fv-az714-382:09069] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f9a142ae277]
[fv-az714-382:09069] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9a142ae52b]
[fv-az714-382:09069] [ 8] plumed(+0x12f48)[0x55c4823c2f48]
[fv-az714-382:09069] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9a13e29d90]
[fv-az714-382:09069] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9a13e29e40]
[fv-az714-382:09069] [11] plumed(+0x131e5)[0x55c4823c31e5]
[fv-az714-382:09069] *** End of error message ***
</pre>
{% endraw %}

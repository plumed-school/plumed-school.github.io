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
[fv-az659-187:42055] *** Process received signal ***
[fv-az659-187:42055] Signal: Aborted (6)
[fv-az659-187:42055] Signal code:  (-6)
[fv-az659-187:42055] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5b3f642520]
[fv-az659-187:42055] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5b3f6969fc]
[fv-az659-187:42055] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5b3f642476]
[fv-az659-187:42055] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5b3f6287f3]
[fv-az659-187:42055] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f5b3faa2b9e]
[fv-az659-187:42055] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f5b3faae20c]
[fv-az659-187:42055] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f5b3faae277]
[fv-az659-187:42055] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f5b3faae52b]
[fv-az659-187:42055] [ 8] plumed(+0x12f48)[0x5635c2dd3f48]
[fv-az659-187:42055] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5b3f629d90]
[fv-az659-187:42055] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5b3f629e40]
[fv-az659-187:42055] [11] plumed(+0x131e5)[0x5635c2dd41e5]
[fv-az659-187:42055] *** End of error message ***
</pre>
{% endraw %}

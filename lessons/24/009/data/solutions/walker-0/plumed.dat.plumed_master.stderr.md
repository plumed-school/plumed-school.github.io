Stderr for source:  ./solutions/walker-0/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action HBOND_MATRIX with label hbmat1 : cannot understand the following words from the input line : SUM
[fv-az740-873:41201] *** Process received signal ***
[fv-az740-873:41201] Signal: Aborted (6)
[fv-az740-873:41201] Signal code:  (-6)
[fv-az740-873:41201] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f82b0242520]
[fv-az740-873:41201] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f82b02969fc]
[fv-az740-873:41201] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f82b0242476]
[fv-az740-873:41201] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f82b02287f3]
[fv-az740-873:41201] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f82b06a2b9e]
[fv-az740-873:41201] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f82b06ae20c]
[fv-az740-873:41201] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f82b06ae277]
[fv-az740-873:41201] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f82b06ae52b]
[fv-az740-873:41201] [ 8] plumed_master(+0x14274)[0x562fcb5e1274]
[fv-az740-873:41201] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f82b0229d90]
[fv-az740-873:41201] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f82b0229e40]
[fv-az740-873:41201] [11] plumed_master(+0x14ed5)[0x562fcb5e1ed5]
[fv-az740-873:41201] *** End of error message ***
</pre>
{% endraw %}

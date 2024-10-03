Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label s : keyword SIGMA could not be read correctly
[fv-az740-873:42065] *** Process received signal ***
[fv-az740-873:42065] Signal: Aborted (6)
[fv-az740-873:42065] Signal code:  (-6)
[fv-az740-873:42065] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f55da242520]
[fv-az740-873:42065] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f55da2969fc]
[fv-az740-873:42065] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f55da242476]
[fv-az740-873:42065] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f55da2287f3]
[fv-az740-873:42065] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f55da6a2b9e]
[fv-az740-873:42065] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f55da6ae20c]
[fv-az740-873:42065] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f55da6ae277]
[fv-az740-873:42065] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f55da6ae52b]
[fv-az740-873:42065] [ 8] plumed(+0x12f48)[0x55f093528f48]
[fv-az740-873:42065] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f55da229d90]
[fv-az740-873:42065] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f55da229e40]
[fv-az740-873:42065] [11] plumed(+0x131e5)[0x55f0935291e5]
[fv-az740-873:42065] *** End of error message ***
</pre>
{% endraw %}

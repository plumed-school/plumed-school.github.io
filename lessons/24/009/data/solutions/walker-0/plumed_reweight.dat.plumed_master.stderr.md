Stderr for source:  ./solutions/walker-0/plumed_reweight.dat   
Download: [zipped raw stdout](plumed_reweight.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_reweight.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @33 : keyword ARG is compulsory for this action
[fv-az740-873:41232] *** Process received signal ***
[fv-az740-873:41232] Signal: Aborted (6)
[fv-az740-873:41232] Signal code:  (-6)
[fv-az740-873:41232] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd998c42520]
[fv-az740-873:41232] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd998c969fc]
[fv-az740-873:41232] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd998c42476]
[fv-az740-873:41232] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd998c287f3]
[fv-az740-873:41232] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fd9990a2b9e]
[fv-az740-873:41232] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fd9990ae20c]
[fv-az740-873:41232] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fd9990ae277]
[fv-az740-873:41232] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd9990ae52b]
[fv-az740-873:41232] [ 8] plumed_master(+0x14274)[0x55a342757274]
[fv-az740-873:41232] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd998c29d90]
[fv-az740-873:41232] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd998c29e40]
[fv-az740-873:41232] [11] plumed_master(+0x14ed5)[0x55a342757ed5]
[fv-az740-873:41232] *** End of error message ***
</pre>
{% endraw %}

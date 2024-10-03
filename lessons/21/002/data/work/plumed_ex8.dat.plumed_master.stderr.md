Stderr for source:  work/plumed_ex8.dat   
Download: [zipped raw stdout](plumed_ex8.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex8.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @49 : keyword ARG is compulsory for this action
[fv-az1205-759:42363] *** Process received signal ***
[fv-az1205-759:42363] Signal: Aborted (6)
[fv-az1205-759:42363] Signal code:  (-6)
[fv-az1205-759:42363] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f4626c42520]
[fv-az1205-759:42363] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f4626c969fc]
[fv-az1205-759:42363] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f4626c42476]
[fv-az1205-759:42363] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f4626c287f3]
[fv-az1205-759:42363] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f46270a2b9e]
[fv-az1205-759:42363] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f46270ae20c]
[fv-az1205-759:42363] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f46270ae277]
[fv-az1205-759:42363] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f46270ae52b]
[fv-az1205-759:42363] [ 8] plumed_master(+0x14274)[0x55aff2f75274]
[fv-az1205-759:42363] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f4626c29d90]
[fv-az1205-759:42363] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f4626c29e40]
[fv-az1205-759:42363] [11] plumed_master(+0x14ed5)[0x55aff2f75ed5]
[fv-az1205-759:42363] *** End of error message ***
</pre>
{% endraw %}

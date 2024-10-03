Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(vesselbase/Vessel.cpp:143) void PLMD::vesselbase::Vessel::error(const string&)
ERROR for keyword MORE_THAN in action CLUSTER_DISTRIBUTION with label nclust : could not parse D_0
[fv-az1205-759:41881] *** Process received signal ***
[fv-az1205-759:41881] Signal: Aborted (6)
[fv-az1205-759:41881] Signal code:  (-6)
[fv-az1205-759:41881] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdbb7c42520]
[fv-az1205-759:41881] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdbb7c969fc]
[fv-az1205-759:41881] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdbb7c42476]
[fv-az1205-759:41881] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdbb7c287f3]
[fv-az1205-759:41881] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fdbb80a2b9e]
[fv-az1205-759:41881] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fdbb80ae20c]
[fv-az1205-759:41881] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fdbb80ae277]
[fv-az1205-759:41881] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdbb80ae52b]
[fv-az1205-759:41881] [ 8] plumed(+0x12f48)[0x5636352e3f48]
[fv-az1205-759:41881] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdbb7c29d90]
[fv-az1205-759:41881] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdbb7c29e40]
[fv-az1205-759:41881] [11] plumed(+0x131e5)[0x5636352e41e5]
[fv-az1205-759:41881] *** End of error message ***
</pre>
{% endraw %}

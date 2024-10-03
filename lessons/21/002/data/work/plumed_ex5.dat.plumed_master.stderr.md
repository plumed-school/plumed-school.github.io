Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @12 : keyword ARG is compulsory for this action
[fv-az1205-759:42270] *** Process received signal ***
[fv-az1205-759:42270] Signal: Aborted (6)
[fv-az1205-759:42270] Signal code:  (-6)
[fv-az1205-759:42270] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6a21242520]
[fv-az1205-759:42270] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6a212969fc]
[fv-az1205-759:42270] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6a21242476]
[fv-az1205-759:42270] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6a212287f3]
[fv-az1205-759:42270] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f6a216a2b9e]
[fv-az1205-759:42270] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f6a216ae20c]
[fv-az1205-759:42270] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f6a216ae277]
[fv-az1205-759:42270] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6a216ae52b]
[fv-az1205-759:42270] [ 8] plumed_master(+0x14274)[0x55ed0f4ac274]
[fv-az1205-759:42270] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6a21229d90]
[fv-az1205-759:42270] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6a21229e40]
[fv-az1205-759:42270] [11] plumed_master(+0x14ed5)[0x55ed0f4aced5]
[fv-az1205-759:42270] *** End of error message ***
</pre>
{% endraw %}

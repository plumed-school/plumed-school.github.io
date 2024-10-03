Stderr for source:  work/plumed_ex2.dat   
Download: [zipped raw stdout](plumed_ex2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
WARNING: IFile closed in the middle of reading. seems strange!
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DUMPGRID with label @15 : keyword ARG is compulsory for this action
[fv-az1205-759:42182] *** Process received signal ***
[fv-az1205-759:42182] Signal: Aborted (6)
[fv-az1205-759:42182] Signal code:  (-6)
[fv-az1205-759:42182] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7efd85842520]
[fv-az1205-759:42182] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7efd858969fc]
[fv-az1205-759:42182] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7efd85842476]
[fv-az1205-759:42182] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7efd858287f3]
[fv-az1205-759:42182] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7efd85ca2b9e]
[fv-az1205-759:42182] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7efd85cae20c]
[fv-az1205-759:42182] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7efd85cae277]
[fv-az1205-759:42182] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7efd85cae52b]
[fv-az1205-759:42182] [ 8] plumed_master(+0x14274)[0x557a6bda6274]
[fv-az1205-759:42182] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7efd85829d90]
[fv-az1205-759:42182] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7efd85829e40]
[fv-az1205-759:42182] [11] plumed_master(+0x14ed5)[0x557a6bda6ed5]
[fv-az1205-759:42182] *** End of error message ***
</pre>
{% endraw %}

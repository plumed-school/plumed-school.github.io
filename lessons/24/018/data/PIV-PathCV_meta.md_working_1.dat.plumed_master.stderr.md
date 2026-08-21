Stderr for source:  PIV-PathCV_meta.md_working_1.dat   
Download: [zipped raw stdout](PIV-PathCV_meta.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](PIV-PathCV_meta.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label res : cannot find action named p1 (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[runnervm76f27:04781] *** Process received signal ***
[runnervm76f27:04781] Signal: Aborted (6)
[runnervm76f27:04781] Signal code:  (-6)
[runnervm76f27:04781] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f658b445330]
[runnervm76f27:04781] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f658b49ec0c]
[runnervm76f27:04781] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f658b44527e]
[runnervm76f27:04781] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f658b4288ff]
[runnervm76f27:04781] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f658b8a5ff5]
[runnervm76f27:04781] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f658b8bb0da]
[runnervm76f27:04781] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f658b8a5a55]
[runnervm76f27:04781] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f658b8a5a6f]
[runnervm76f27:04781] [ 8] plumed_master(+0x146dd)[0x5558a46826dd]
[runnervm76f27:04781] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f658b42a1ca]
[runnervm76f27:04781] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f658b42a28b]
[runnervm76f27:04781] [11] plumed_master(+0x15365)[0x5558a4683365]
[runnervm76f27:04781] *** End of error message ***
</pre>
{% endraw %}

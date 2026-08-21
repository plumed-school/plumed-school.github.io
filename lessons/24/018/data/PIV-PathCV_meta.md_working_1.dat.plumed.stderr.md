Stderr for source:  PIV-PathCV_meta.md_working_1.dat   
Download: [zipped raw stdout](PIV-PathCV_meta.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](PIV-PathCV_meta.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label res : cannot find action named p1 (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[runnervm76f27:04765] *** Process received signal ***
[runnervm76f27:04765] Signal: Aborted (6)
[runnervm76f27:04765] Signal code:  (-6)
[runnervm76f27:04765] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f9bad045330]
[runnervm76f27:04765] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f9bad09ec0c]
[runnervm76f27:04765] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f9bad04527e]
[runnervm76f27:04765] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f9bad0288ff]
[runnervm76f27:04765] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f9bad4a5ff5]
[runnervm76f27:04765] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f9bad4bb0da]
[runnervm76f27:04765] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f9bad4a5a55]
[runnervm76f27:04765] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f9bad4a5a6f]
[runnervm76f27:04765] [ 8] plumed(+0x146dd)[0x5571c48ab6dd]
[runnervm76f27:04765] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f9bad02a1ca]
[runnervm76f27:04765] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f9bad02a28b]
[runnervm76f27:04765] [11] plumed(+0x15365)[0x5571c48ac365]
[runnervm76f27:04765] *** End of error message ***
</pre>
{% endraw %}

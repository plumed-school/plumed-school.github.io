Stderr for source:  INSTRUCTIONS.md_working_7.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: timestep kBT posx posy posz Masses Charges Box driver )
[runnervm76f27:05880] *** Process received signal ***
[runnervm76f27:05880] Signal: Aborted (6)
[runnervm76f27:05880] Signal code:  (-6)
[runnervm76f27:05880] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7eff04a45330]
[runnervm76f27:05880] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7eff04a9ec0c]
[runnervm76f27:05880] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7eff04a4527e]
[runnervm76f27:05880] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7eff04a288ff]
[runnervm76f27:05880] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7eff04ea5ff5]
[runnervm76f27:05880] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7eff04ebb0da]
[runnervm76f27:05880] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7eff04ea5a55]
[runnervm76f27:05880] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7eff04ea5a6f]
[runnervm76f27:05880] [ 8] plumed(+0x146dd)[0x5594cf9b26dd]
[runnervm76f27:05880] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7eff04a2a1ca]
[runnervm76f27:05880] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7eff04a2a28b]
[runnervm76f27:05880] [11] plumed(+0x15365)[0x5594cf9b3365]
[runnervm76f27:05880] *** End of error message ***
</pre>
{% endraw %}

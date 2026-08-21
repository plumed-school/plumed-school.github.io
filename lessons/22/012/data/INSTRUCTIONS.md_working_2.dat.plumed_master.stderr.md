Stderr for source:  INSTRUCTIONS.md_working_2.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:372) void PLMD::Action::error(const std::string&) const
ERROR in input to action ENVIRONMENTSIMILARITY with label @s9 : keyword SIGMA could not be read correctly
[runnervm76f27:05698] *** Process received signal ***
[runnervm76f27:05698] Signal: Aborted (6)
[runnervm76f27:05698] Signal code:  (-6)
[runnervm76f27:05698] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fb39b845330]
[runnervm76f27:05698] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fb39b89ec0c]
[runnervm76f27:05698] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fb39b84527e]
[runnervm76f27:05698] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fb39b8288ff]
[runnervm76f27:05698] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fb39bca5ff5]
[runnervm76f27:05698] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fb39bcbb0da]
[runnervm76f27:05698] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fb39bca5a55]
[runnervm76f27:05698] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fb39bca5a6f]
[runnervm76f27:05698] [ 8] plumed_master(+0x146dd)[0x5644722366dd]
[runnervm76f27:05698] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fb39b82a1ca]
[runnervm76f27:05698] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fb39b82a28b]
[runnervm76f27:05698] [11] plumed_master(+0x15365)[0x564472237365]
[runnervm76f27:05698] *** End of error message ***
</pre>
{% endraw %}

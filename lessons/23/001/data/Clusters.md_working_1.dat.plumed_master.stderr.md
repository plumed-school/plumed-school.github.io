Stderr for source:  Clusters.md_working_1.dat   
Download: [zipped raw stdout](Clusters.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](Clusters.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:309) void PLMD::Action::error(const string&) const
ERROR in input to action DFSCLUSTERING with label dfs : keyword ARG is compulsory for this action
[fv-az714-650:44016] *** Process received signal ***
[fv-az714-650:44016] Signal: Aborted (6)
[fv-az714-650:44016] Signal code:  (-6)
[fv-az714-650:44016] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe5f7c42520]
[fv-az714-650:44016] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe5f7c969fc]
[fv-az714-650:44016] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe5f7c42476]
[fv-az714-650:44016] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe5f7c287f3]
[fv-az714-650:44016] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fe5f80a2b9e]
[fv-az714-650:44016] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fe5f80ae20c]
[fv-az714-650:44016] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fe5f80ae277]
[fv-az714-650:44016] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe5f80ae52b]
[fv-az714-650:44016] [ 8] plumed_master(+0x14274)[0x5585b05a9274]
[fv-az714-650:44016] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe5f7c29d90]
[fv-az714-650:44016] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe5f7c29e40]
[fv-az714-650:44016] [11] plumed_master(+0x14ed5)[0x5585b05a9ed5]
[fv-az714-650:44016] *** End of error message ***
</pre>
{% endraw %}

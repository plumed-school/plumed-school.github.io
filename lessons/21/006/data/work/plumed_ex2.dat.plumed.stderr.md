Stderr for source:  work/plumed_ex2.dat   
Download: [zipped raw stdout](plumed_ex2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action PCA with label pca : action cc has no component named cc (hint! the components in this actions are: )
[fv-az714-382:09039] *** Process received signal ***
[fv-az714-382:09039] Signal: Aborted (6)
[fv-az714-382:09039] Signal code:  (-6)
[fv-az714-382:09039] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8230442520]
[fv-az714-382:09039] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f82304969fc]
[fv-az714-382:09039] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8230442476]
[fv-az714-382:09039] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f82304287f3]
[fv-az714-382:09039] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f82308a2b9e]
[fv-az714-382:09039] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f82308ae20c]
[fv-az714-382:09039] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f82308ae277]
[fv-az714-382:09039] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f82308ae52b]
[fv-az714-382:09039] [ 8] plumed(+0x12f48)[0x558ff4a60f48]
[fv-az714-382:09039] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8230429d90]
[fv-az714-382:09039] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8230429e40]
[fv-az714-382:09039] [11] plumed(+0x131e5)[0x558ff4a611e5]
[fv-az714-382:09039] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  Clusters.md_working_2.dat   
Download: [zipped raw stdout](Clusters.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Clusters.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cm : No atoms have been read in
[fv-az714-382:08239] *** Process received signal ***
[fv-az714-382:08239] Signal: Aborted (6)
[fv-az714-382:08239] Signal code:  (-6)
[fv-az714-382:08239] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc1d4c42520]
[fv-az714-382:08239] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc1d4c969fc]
[fv-az714-382:08239] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc1d4c42476]
[fv-az714-382:08239] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc1d4c287f3]
[fv-az714-382:08239] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc1d50a2b9e]
[fv-az714-382:08239] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc1d50ae20c]
[fv-az714-382:08239] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc1d50ae277]
[fv-az714-382:08239] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc1d50ae52b]
[fv-az714-382:08239] [ 8] plumed(+0x12f48)[0x55c24945ff48]
[fv-az714-382:08239] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc1d4c29d90]
[fv-az714-382:08239] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc1d4c29e40]
[fv-az714-382:08239] [11] plumed(+0x131e5)[0x55c2494601e5]
[fv-az714-382:08239] *** End of error message ***
</pre>
{% endraw %}

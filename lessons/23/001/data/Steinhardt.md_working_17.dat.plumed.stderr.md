Stderr for source:  Steinhardt.md_working_17.dat   
Download: [zipped raw stdout](Steinhardt.md_working_17.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_17.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az714-382:06889] *** Process received signal ***
[fv-az714-382:06889] Signal: Aborted (6)
[fv-az714-382:06889] Signal code:  (-6)
[fv-az714-382:06889] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1f33442520]
[fv-az714-382:06889] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1f334969fc]
[fv-az714-382:06889] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1f33442476]
[fv-az714-382:06889] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1f334287f3]
[fv-az714-382:06889] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1f338a2b9e]
[fv-az714-382:06889] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1f338ae20c]
[fv-az714-382:06889] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1f338ae277]
[fv-az714-382:06889] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1f338ae52b]
[fv-az714-382:06889] [ 8] plumed(+0x12f48)[0x55e88dbaff48]
[fv-az714-382:06889] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1f33429d90]
[fv-az714-382:06889] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1f33429e40]
[fv-az714-382:06889] [11] plumed(+0x131e5)[0x55e88dbb01e5]
[fv-az714-382:06889] *** End of error message ***
</pre>
{% endraw %}

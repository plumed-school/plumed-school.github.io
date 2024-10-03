Stderr for source:  Steinhardt.md_working_18.dat   
Download: [zipped raw stdout](Steinhardt.md_working_18.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Steinhardt.md_working_18.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az714-650:42732] *** Process received signal ***
[fv-az714-650:42732] Signal: Aborted (6)
[fv-az714-650:42732] Signal code:  (-6)
[fv-az714-650:42732] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fb304042520]
[fv-az714-650:42732] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fb3040969fc]
[fv-az714-650:42732] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fb304042476]
[fv-az714-650:42732] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fb3040287f3]
[fv-az714-650:42732] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fb3044a2b9e]
[fv-az714-650:42732] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fb3044ae20c]
[fv-az714-650:42732] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fb3044ae277]
[fv-az714-650:42732] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fb3044ae52b]
[fv-az714-650:42732] [ 8] plumed(+0x12f48)[0x56360b3cbf48]
[fv-az714-650:42732] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fb304029d90]
[fv-az714-650:42732] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fb304029e40]
[fv-az714-650:42732] [11] plumed(+0x131e5)[0x56360b3cc1e5]
[fv-az714-650:42732] *** End of error message ***
</pre>
{% endraw %}

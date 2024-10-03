Stderr for source:  Volumes.md_working_3.dat   
Download: [zipped raw stdout](Volumes.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Volumes.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label cmat : No atoms have been read in
[fv-az714-650:43038] *** Process received signal ***
[fv-az714-650:43038] Signal: Aborted (6)
[fv-az714-650:43038] Signal code:  (-6)
[fv-az714-650:43038] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6732e42520]
[fv-az714-650:43038] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6732e969fc]
[fv-az714-650:43038] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6732e42476]
[fv-az714-650:43038] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6732e287f3]
[fv-az714-650:43038] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f67332a2b9e]
[fv-az714-650:43038] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f67332ae20c]
[fv-az714-650:43038] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f67332ae277]
[fv-az714-650:43038] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f67332ae52b]
[fv-az714-650:43038] [ 8] plumed(+0x12f48)[0x562ffc6eaf48]
[fv-az714-650:43038] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6732e29d90]
[fv-az714-650:43038] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6732e29e40]
[fv-az714-650:43038] [11] plumed(+0x131e5)[0x562ffc6eb1e5]
[fv-az714-650:43038] *** End of error message ***
</pre>
{% endraw %}

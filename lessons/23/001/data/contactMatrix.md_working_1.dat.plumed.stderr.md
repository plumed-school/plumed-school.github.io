Stderr for source:  contactMatrix.md_working_1.dat   
Download: [zipped raw stdout](contactMatrix.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-650:41666] *** Process received signal ***
[fv-az714-650:41666] Signal: Aborted (6)
[fv-az714-650:41666] Signal code:  (-6)
[fv-az714-650:41666] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fae4ca42520]
[fv-az714-650:41666] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fae4ca969fc]
[fv-az714-650:41666] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fae4ca42476]
[fv-az714-650:41666] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fae4ca287f3]
[fv-az714-650:41666] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fae4cea2b9e]
[fv-az714-650:41666] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fae4ceae20c]
[fv-az714-650:41666] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fae4ceae277]
[fv-az714-650:41666] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fae4ceae52b]
[fv-az714-650:41666] [ 8] plumed(+0x12f48)[0x55e193731f48]
[fv-az714-650:41666] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fae4ca29d90]
[fv-az714-650:41666] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fae4ca29e40]
[fv-az714-650:41666] [11] plumed(+0x131e5)[0x55e1937321e5]
[fv-az714-650:41666] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  contactMatrix.md_working_4.dat   
Download: [zipped raw stdout](contactMatrix.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-650:41789] *** Process received signal ***
[fv-az714-650:41789] Signal: Aborted (6)
[fv-az714-650:41789] Signal code:  (-6)
[fv-az714-650:41789] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9cc2042520]
[fv-az714-650:41789] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9cc20969fc]
[fv-az714-650:41789] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9cc2042476]
[fv-az714-650:41789] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9cc20287f3]
[fv-az714-650:41789] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f9cc24a2b9e]
[fv-az714-650:41789] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f9cc24ae20c]
[fv-az714-650:41789] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f9cc24ae277]
[fv-az714-650:41789] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f9cc24ae52b]
[fv-az714-650:41789] [ 8] plumed(+0x12f48)[0x561a266d0f48]
[fv-az714-650:41789] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9cc2029d90]
[fv-az714-650:41789] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9cc2029e40]
[fv-az714-650:41789] [11] plumed(+0x131e5)[0x561a266d11e5]
[fv-az714-650:41789] *** End of error message ***
</pre>
{% endraw %}

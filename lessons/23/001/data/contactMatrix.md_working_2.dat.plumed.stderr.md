Stderr for source:  contactMatrix.md_working_2.dat   
Download: [zipped raw stdout](contactMatrix.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](contactMatrix.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action CONTACT_MATRIX with label c1 : No atoms have been read in
[fv-az714-382:05866] *** Process received signal ***
[fv-az714-382:05866] Signal: Aborted (6)
[fv-az714-382:05866] Signal code:  (-6)
[fv-az714-382:05866] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8939a42520]
[fv-az714-382:05866] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8939a969fc]
[fv-az714-382:05866] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8939a42476]
[fv-az714-382:05866] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8939a287f3]
[fv-az714-382:05866] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8939ea2b9e]
[fv-az714-382:05866] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8939eae20c]
[fv-az714-382:05866] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8939eae277]
[fv-az714-382:05866] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8939eae52b]
[fv-az714-382:05866] [ 8] plumed(+0x12f48)[0x556c7cd8df48]
[fv-az714-382:05866] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8939a29d90]
[fv-az714-382:05866] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8939a29e40]
[fv-az714-382:05866] [11] plumed(+0x131e5)[0x556c7cd8e1e5]
[fv-az714-382:05866] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  INSTRUCTIONS.md_working_4.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_4.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_4.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az714-382:08950] *** Process received signal ***
[fv-az714-382:08950] Signal: Aborted (6)
[fv-az714-382:08950] Signal code:  (-6)
[fv-az714-382:08950] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8a42a42520]
[fv-az714-382:08950] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8a42a969fc]
[fv-az714-382:08950] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8a42a42476]
[fv-az714-382:08950] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8a42a287f3]
[fv-az714-382:08950] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f8a42ea2b9e]
[fv-az714-382:08950] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f8a42eae20c]
[fv-az714-382:08950] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f8a42eae277]
[fv-az714-382:08950] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f8a42eae52b]
[fv-az714-382:08950] [ 8] plumed_master(+0x14274)[0x563c1bd33274]
[fv-az714-382:08950] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8a42a29d90]
[fv-az714-382:08950] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8a42a29e40]
[fv-az714-382:08950] [11] plumed_master(+0x14ed5)[0x563c1bd33ed5]
[fv-az714-382:08950] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  INSTRUCTIONS.md_working_3.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az714-382:08919] *** Process received signal ***
[fv-az714-382:08919] Signal: Aborted (6)
[fv-az714-382:08919] Signal code:  (-6)
[fv-az714-382:08919] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1c8a042520]
[fv-az714-382:08919] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f1c8a0969fc]
[fv-az714-382:08919] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1c8a042476]
[fv-az714-382:08919] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f1c8a0287f3]
[fv-az714-382:08919] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f1c8a4a2b9e]
[fv-az714-382:08919] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f1c8a4ae20c]
[fv-az714-382:08919] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f1c8a4ae277]
[fv-az714-382:08919] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f1c8a4ae52b]
[fv-az714-382:08919] [ 8] plumed_master(+0x14274)[0x555ed168b274]
[fv-az714-382:08919] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1c8a029d90]
[fv-az714-382:08919] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1c8a029e40]
[fv-az714-382:08919] [11] plumed_master(+0x14ed5)[0x555ed168bed5]
[fv-az714-382:08919] *** End of error message ***
</pre>
{% endraw %}

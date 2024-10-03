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
[fv-az1205-759:41956] *** Process received signal ***
[fv-az1205-759:41956] Signal: Aborted (6)
[fv-az1205-759:41956] Signal code:  (-6)
[fv-az1205-759:41956] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f2590c42520]
[fv-az1205-759:41956] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f2590c969fc]
[fv-az1205-759:41956] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f2590c42476]
[fv-az1205-759:41956] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f2590c287f3]
[fv-az1205-759:41956] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f25910a2b9e]
[fv-az1205-759:41956] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f25910ae20c]
[fv-az1205-759:41956] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f25910ae277]
[fv-az1205-759:41956] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f25910ae52b]
[fv-az1205-759:41956] [ 8] plumed_master(+0x14274)[0x55ff89d03274]
[fv-az1205-759:41956] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f2590c29d90]
[fv-az1205-759:41956] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f2590c29e40]
[fv-az1205-759:41956] [11] plumed_master(+0x14ed5)[0x55ff89d03ed5]
[fv-az1205-759:41956] *** End of error message ***
</pre>
{% endraw %}

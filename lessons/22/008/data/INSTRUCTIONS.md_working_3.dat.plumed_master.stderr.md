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
[fv-az1106-805:42883] *** Process received signal ***
[fv-az1106-805:42883] Signal: Aborted (6)
[fv-az1106-805:42883] Signal code:  (-6)
[fv-az1106-805:42883] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ffbb7842520]
[fv-az1106-805:42883] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ffbb78969fc]
[fv-az1106-805:42883] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ffbb7842476]
[fv-az1106-805:42883] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ffbb78287f3]
[fv-az1106-805:42883] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ffbb7ca2b9e]
[fv-az1106-805:42883] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ffbb7cae20c]
[fv-az1106-805:42883] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ffbb7cae277]
[fv-az1106-805:42883] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ffbb7cae52b]
[fv-az1106-805:42883] [ 8] plumed_master(+0x14274)[0x55a726fc1274]
[fv-az1106-805:42883] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ffbb7829d90]
[fv-az1106-805:42883] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ffbb7829e40]
[fv-az1106-805:42883] [11] plumed_master(+0x14ed5)[0x55a726fc1ed5]
[fv-az1106-805:42883] *** End of error message ***
</pre>
{% endraw %}

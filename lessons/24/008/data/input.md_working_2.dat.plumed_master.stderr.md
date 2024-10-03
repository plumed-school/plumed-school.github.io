Stderr for source:  input.md_working_2.dat   
Download: [zipped raw stdout](input.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](input.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/RegisterBase.h:211) const Content& PLMD::RegisterBase<Content>::get(const std::vector<void*>&, const string&) const [with Content = PLMD::ActionRegisterPointers; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: m.count(key)>0
[fv-az659-187:41245] *** Process received signal ***
[fv-az659-187:41245] Signal: Aborted (6)
[fv-az659-187:41245] Signal code:  (-6)
[fv-az659-187:41245] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f17f1642520]
[fv-az659-187:41245] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f17f16969fc]
[fv-az659-187:41245] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f17f1642476]
[fv-az659-187:41245] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f17f16287f3]
[fv-az659-187:41245] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f17f1aa2b9e]
[fv-az659-187:41245] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f17f1aae20c]
[fv-az659-187:41245] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f17f1aae277]
[fv-az659-187:41245] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f17f1aae52b]
[fv-az659-187:41245] [ 8] plumed_master(+0x14274)[0x55ac60710274]
[fv-az659-187:41245] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f17f1629d90]
[fv-az659-187:41245] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f17f1629e40]
[fv-az659-187:41245] [11] plumed_master(+0x14ed5)[0x55ac60710ed5]
[fv-az659-187:41245] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  this_input_should_work.dat   
Download: [zipped raw stdout](this_input_should_work.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](this_input_should_work.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:984) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&, const bool&)
ERROR
I cannot understand line: CONTACT_MATIX LABEL=cm ATOMS=1-100 SWITCH=CUBIC D_0=0.45 D_MAX=0.55
Maybe a missing space or a typo?
[fv-az523-443:66733] *** Process received signal ***
[fv-az523-443:66733] Signal: Aborted (6)
[fv-az523-443:66733] Signal code:  (-6)
[fv-az523-443:66733] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa642042520]
[fv-az523-443:66733] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa6420969fc]
[fv-az523-443:66733] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa642042476]
[fv-az523-443:66733] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa6420287f3]
[fv-az523-443:66733] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fa6424a4f26]
[fv-az523-443:66733] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fa6424b6d9c]
[fv-az523-443:66733] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fa6424b6e07]
[fv-az523-443:66733] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa6424b70bb]
[fv-az523-443:66733] [ 8] plumed_master(+0x12e7f)[0x5608c76b1e7f]
[fv-az523-443:66733] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa642029d90]
[fv-az523-443:66733] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa642029e40]
[fv-az523-443:66733] [11] plumed_master(+0x13115)[0x5608c76b2115]
[fv-az523-443:66733] *** End of error message ***
</pre>
{% endraw %}

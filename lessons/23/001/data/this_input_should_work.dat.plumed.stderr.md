Stderr for source:  this_input_should_work.dat   
Download: [zipped raw stdout](this_input_should_work.dat.plumed.stdout.txt.zip) - [zipped raw stderr](this_input_should_work.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:823) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: CONTACT_MATIX LABEL=cm ATOMS=1-100 SWITCH=CUBIC D_0=0.45 D_MAX=0.55
Maybe a missing space or a typo?
[fv-az523-443:66725] *** Process received signal ***
[fv-az523-443:66725] Signal: Aborted (6)
[fv-az523-443:66725] Signal code:  (-6)
[fv-az523-443:66725] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fe36e242520]
[fv-az523-443:66725] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fe36e2969fc]
[fv-az523-443:66725] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fe36e242476]
[fv-az523-443:66725] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fe36e2287f3]
[fv-az523-443:66725] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fe36e6a4f26]
[fv-az523-443:66725] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fe36e6b6d9c]
[fv-az523-443:66725] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fe36e6b6e07]
[fv-az523-443:66725] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fe36e6b70bb]
[fv-az523-443:66725] [ 8] plumed(+0x12f48)[0x558b45ac8f48]
[fv-az523-443:66725] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fe36e229d90]
[fv-az523-443:66725] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fe36e229e40]
[fv-az523-443:66725] [11] plumed(+0x131e5)[0x558b45ac91e5]
[fv-az523-443:66725] *** End of error message ***
</pre>
{% endraw %}

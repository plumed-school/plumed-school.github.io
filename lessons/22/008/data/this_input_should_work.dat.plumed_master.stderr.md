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
I cannot understand line: CMUMD LABEL=left GROUP=lj NSV=1 FIXED=0.4 DCR=0.25 CRSIZE=0.1 WF=0.0001 ASYMM=-1 NINT=0.1 NZ=291
Maybe a missing space or a typo?
[fv-az523-443:67104] *** Process received signal ***
[fv-az523-443:67104] Signal: Aborted (6)
[fv-az523-443:67104] Signal code:  (-6)
[fv-az523-443:67104] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fdd15642520]
[fv-az523-443:67104] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fdd156969fc]
[fv-az523-443:67104] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fdd15642476]
[fv-az523-443:67104] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fdd156287f3]
[fv-az523-443:67104] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fdd15aa4f26]
[fv-az523-443:67104] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fdd15ab6d9c]
[fv-az523-443:67104] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fdd15ab6e07]
[fv-az523-443:67104] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fdd15ab70bb]
[fv-az523-443:67104] [ 8] plumed_master(+0x12e7f)[0x558864654e7f]
[fv-az523-443:67104] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fdd15629d90]
[fv-az523-443:67104] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fdd15629e40]
[fv-az523-443:67104] [11] plumed_master(+0x13115)[0x558864655115]
[fv-az523-443:67104] *** End of error message ***
</pre>
{% endraw %}

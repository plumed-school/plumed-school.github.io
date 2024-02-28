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
I cannot understand line: CMUMD LABEL=left GROUP=lj NSV=1 FIXED=0.4 DCR=0.25 CRSIZE=0.1 WF=0.0001 ASYMM=-1 NINT=0.1 NZ=291
Maybe a missing space or a typo?
[fv-az523-443:67096] *** Process received signal ***
[fv-az523-443:67096] Signal: Aborted (6)
[fv-az523-443:67096] Signal code:  (-6)
[fv-az523-443:67096] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f6f79442520]
[fv-az523-443:67096] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f6f794969fc]
[fv-az523-443:67096] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f6f79442476]
[fv-az523-443:67096] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f6f794287f3]
[fv-az523-443:67096] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7f6f798a4f26]
[fv-az523-443:67096] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7f6f798b6d9c]
[fv-az523-443:67096] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7f6f798b6e07]
[fv-az523-443:67096] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f6f798b70bb]
[fv-az523-443:67096] [ 8] plumed(+0x12f48)[0x56256ce6ef48]
[fv-az523-443:67096] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f6f79429d90]
[fv-az523-443:67096] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f6f79429e40]
[fv-az523-443:67096] [11] plumed(+0x131e5)[0x56256ce6f1e5]
[fv-az523-443:67096] *** End of error message ***
</pre>
{% endraw %}

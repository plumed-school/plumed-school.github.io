Stderr for source:  INSTRUCTIONS.md_working_3.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_3.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: CMUMD LABEL=left GROUP=lj NSV=1 FIXED=0.5 DCR=0.25 CRSIZE=0.1 WF=0.0001 ASYMM=-1 NINT=0.1 NZ=291
Maybe a missing space or a typo?
[fv-az1205-759:41914] *** Process received signal ***
[fv-az1205-759:41914] Signal: Aborted (6)
[fv-az1205-759:41914] Signal code:  (-6)
[fv-az1205-759:41914] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9246042520]
[fv-az1205-759:41914] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f92460969fc]
[fv-az1205-759:41914] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9246042476]
[fv-az1205-759:41914] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f92460287f3]
[fv-az1205-759:41914] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f92464a2b9e]
[fv-az1205-759:41914] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f92464ae20c]
[fv-az1205-759:41914] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f92464ae277]
[fv-az1205-759:41914] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f92464ae52b]
[fv-az1205-759:41914] [ 8] plumed(+0x12f48)[0x5610a57ebf48]
[fv-az1205-759:41914] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9246029d90]
[fv-az1205-759:41914] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9246029e40]
[fv-az1205-759:41914] [11] plumed(+0x131e5)[0x5610a57ec1e5]
[fv-az1205-759:41914] *** End of error message ***
</pre>
{% endraw %}

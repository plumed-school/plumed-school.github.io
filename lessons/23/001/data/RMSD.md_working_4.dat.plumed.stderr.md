Stderr for source:  RMSD.md_working_4.dat   
Download: [zipped raw stdout](RMSD.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](RMSD.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(reference/MetricRegister.h:103) std::unique_ptr<_Tp> PLMD::MetricRegister::create(const string&, const PLMD::PDB&) [with T = PLMD::ReferenceConfiguration; std::string = std::__cxx11::basic_string<char>]
+++ assertion failed: rtype.length()>0
TYPE not specified in pdb input file
[fv-az714-650:44192] *** Process received signal ***
[fv-az714-650:44192] Signal: Aborted (6)
[fv-az714-650:44192] Signal code:  (-6)
[fv-az714-650:44192] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8610442520]
[fv-az714-650:44192] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f86104969fc]
[fv-az714-650:44192] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8610442476]
[fv-az714-650:44192] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f86104287f3]
[fv-az714-650:44192] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f86108a2b9e]
[fv-az714-650:44192] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f86108ae20c]
[fv-az714-650:44192] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f86108ae277]
[fv-az714-650:44192] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f86108ae52b]
[fv-az714-650:44192] [ 8] plumed(+0x12f48)[0x56044c804f48]
[fv-az714-650:44192] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f8610429d90]
[fv-az714-650:44192] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f8610429e40]
[fv-az714-650:44192] [11] plumed(+0x131e5)[0x56044c8051e5]
[fv-az714-650:44192] *** End of error message ***
</pre>
{% endraw %}

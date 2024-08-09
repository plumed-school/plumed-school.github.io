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
[fv-az714-382:08391] *** Process received signal ***
[fv-az714-382:08391] Signal: Aborted (6)
[fv-az714-382:08391] Signal code:  (-6)
[fv-az714-382:08391] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7d19242520]
[fv-az714-382:08391] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7d192969fc]
[fv-az714-382:08391] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7d19242476]
[fv-az714-382:08391] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7d192287f3]
[fv-az714-382:08391] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f7d196a2b9e]
[fv-az714-382:08391] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f7d196ae20c]
[fv-az714-382:08391] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f7d196ae277]
[fv-az714-382:08391] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f7d196ae52b]
[fv-az714-382:08391] [ 8] plumed(+0x12f48)[0x558600836f48]
[fv-az714-382:08391] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7d19229d90]
[fv-az714-382:08391] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7d19229e40]
[fv-az714-382:08391] [11] plumed(+0x131e5)[0x5586008371e5]
[fv-az714-382:08391] *** End of error message ***
</pre>
{% endraw %}

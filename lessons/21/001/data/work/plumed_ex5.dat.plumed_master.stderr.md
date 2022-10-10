Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
+++ PLUMED error
+++ message follows +++

+++ PLUMED error
+++ at GenericMolInfo.cpp:278, function void PLMD::GenericMolInfo::interpretSymbol(const string&, std::vector<PLMD::AtomNumber>&)
+++ message follows +++
Error importing MDAnalysis module: No module named 'MDAnalysis'
[fv-az457-184:06325] *** Process received signal ***
[fv-az457-184:06325] Signal: Aborted (6)
[fv-az457-184:06325] Signal code:  (-6)
[fv-az457-184:06325] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x43090)[0x7f0abf68c090]
[fv-az457-184:06325] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f0abf68c00b]
[fv-az457-184:06325] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f0abf66b859]
[fv-az457-184:06325] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e911)[0x7f0abf8f6911]
[fv-az457-184:06325] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa38c)[0x7f0abf90238c]
[fv-az457-184:06325] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa3f7)[0x7f0abf9023f7]
[fv-az457-184:06325] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f0abf9026fd]
[fv-az457-184:06325] [ 7] plumed_master(+0xf5e9)[0x561160de45e9]
[fv-az457-184:06325] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f0abf66d083]
[fv-az457-184:06325] [ 9] plumed_master(+0xf86e)[0x561160de486e]
[fv-az457-184:06325] *** End of error message ***
</pre>
{% endraw %}

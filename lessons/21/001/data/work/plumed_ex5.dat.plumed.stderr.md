Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::Exception'
what():
+++ PLUMED error
+++ message follows +++

+++ PLUMED error
+++ at GenericMolInfo.cpp:238, function void PLMD::GenericMolInfo::interpretSymbol(const string&, std::vector<PLMD::AtomNumber>&)
+++ message follows +++
Error importing MDAnalysis module: No module named 'MDAnalysis'
[fv-az457-184:06311] *** Process received signal ***
[fv-az457-184:06311] Signal: Aborted (6)
[fv-az457-184:06311] Signal code:  (-6)
[fv-az457-184:06311] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x43090)[0x7f5350e69090]
[fv-az457-184:06311] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f5350e6900b]
[fv-az457-184:06311] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f5350e48859]
[fv-az457-184:06311] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e911)[0x7f53510d3911]
[fv-az457-184:06311] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa38c)[0x7f53510df38c]
[fv-az457-184:06311] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa3f7)[0x7f53510df3f7]
[fv-az457-184:06311] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f53510df6fd]
[fv-az457-184:06311] [ 7] plumed(+0xf5c9)[0x55a92673e5c9]
[fv-az457-184:06311] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f5350e4a083]
[fv-az457-184:06311] [ 9] plumed(+0xf84e)[0x55a92673e84e]
[fv-az457-184:06311] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed.stderr.txt.zip) 
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
[fv-az457-184:06238] *** Process received signal ***
[fv-az457-184:06238] Signal: Aborted (6)
[fv-az457-184:06238] Signal code:  (-6)
[fv-az457-184:06238] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x43090)[0x7f4780906090]
[fv-az457-184:06238] [ 1] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0xcb)[0x7f478090600b]
[fv-az457-184:06238] [ 2] /lib/x86_64-linux-gnu/libc.so.6(abort+0x12b)[0x7f47808e5859]
[fv-az457-184:06238] [ 3] /lib/x86_64-linux-gnu/libstdc++.so.6(+0x9e911)[0x7f4780b70911]
[fv-az457-184:06238] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa38c)[0x7f4780b7c38c]
[fv-az457-184:06238] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xaa3f7)[0x7f4780b7c3f7]
[fv-az457-184:06238] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4d)[0x7f4780b7c6fd]
[fv-az457-184:06238] [ 7] plumed(+0xf5c9)[0x55f56662d5c9]
[fv-az457-184:06238] [ 8] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0xf3)[0x7f47808e7083]
[fv-az457-184:06238] [ 9] plumed(+0xf84e)[0x55f56662d84e]
[fv-az457-184:06238] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  INSTRUCTIONS.md_working_1.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:124) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[fv-az1205-759:42109] *** Process received signal ***
[fv-az1205-759:42109] Signal: Aborted (6)
[fv-az1205-759:42109] Signal code:  (-6)
[fv-az1205-759:42109] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3a1d042520]
[fv-az1205-759:42109] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3a1d0969fc]
[fv-az1205-759:42109] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3a1d042476]
[fv-az1205-759:42109] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3a1d0287f3]
[fv-az1205-759:42109] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3a1d4a2b9e]
[fv-az1205-759:42109] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3a1d4ae20c]
[fv-az1205-759:42109] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3a1d4ae277]
[fv-az1205-759:42109] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3a1d4ae52b]
[fv-az1205-759:42109] [ 8] plumed(+0x12f48)[0x556362032f48]
[fv-az1205-759:42109] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3a1d029d90]
[fv-az1205-759:42109] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3a1d029e40]
[fv-az1205-759:42109] [11] plumed(+0x131e5)[0x5563620331e5]
[fv-az1205-759:42109] *** End of error message ***
</pre>
{% endraw %}

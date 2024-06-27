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
[fv-az1106-805:42939] *** Process received signal ***
[fv-az1106-805:42939] Signal: Aborted (6)
[fv-az1106-805:42939] Signal code:  (-6)
[fv-az1106-805:42939] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3570642520]
[fv-az1106-805:42939] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f35706969fc]
[fv-az1106-805:42939] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3570642476]
[fv-az1106-805:42939] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f35706287f3]
[fv-az1106-805:42939] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3570aa2b9e]
[fv-az1106-805:42939] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3570aae20c]
[fv-az1106-805:42939] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3570aae277]
[fv-az1106-805:42939] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3570aae52b]
[fv-az1106-805:42939] [ 8] plumed(+0x12f48)[0x55ccc3ce8f48]
[fv-az1106-805:42939] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3570629d90]
[fv-az1106-805:42939] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3570629e40]
[fv-az1106-805:42939] [11] plumed(+0x131e5)[0x55ccc3ce91e5]
[fv-az1106-805:42939] *** End of error message ***
</pre>
{% endraw %}

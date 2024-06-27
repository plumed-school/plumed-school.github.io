Stderr for source:  INSTRUCTIONS.md_working_1.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:139) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[fv-az1106-805:42947] *** Process received signal ***
[fv-az1106-805:42947] Signal: Aborted (6)
[fv-az1106-805:42947] Signal code:  (-6)
[fv-az1106-805:42947] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f002d042520]
[fv-az1106-805:42947] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f002d0969fc]
[fv-az1106-805:42947] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f002d042476]
[fv-az1106-805:42947] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f002d0287f3]
[fv-az1106-805:42947] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f002d4a2b9e]
[fv-az1106-805:42947] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f002d4ae20c]
[fv-az1106-805:42947] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f002d4ae277]
[fv-az1106-805:42947] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f002d4ae52b]
[fv-az1106-805:42947] [ 8] plumed_master(+0x14274)[0x559fad28d274]
[fv-az1106-805:42947] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f002d029d90]
[fv-az1106-805:42947] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f002d029e40]
[fv-az1106-805:42947] [11] plumed_master(+0x14ed5)[0x559fad28ded5]
[fv-az1106-805:42947] *** End of error message ***
</pre>
{% endraw %}

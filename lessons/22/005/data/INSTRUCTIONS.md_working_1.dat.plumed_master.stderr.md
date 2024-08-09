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
[fv-az714-382:08983] *** Process received signal ***
[fv-az714-382:08983] Signal: Aborted (6)
[fv-az714-382:08983] Signal code:  (-6)
[fv-az714-382:08983] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f1669042520]
[fv-az714-382:08983] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f16690969fc]
[fv-az714-382:08983] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f1669042476]
[fv-az714-382:08983] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f16690287f3]
[fv-az714-382:08983] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f16694a2b9e]
[fv-az714-382:08983] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f16694ae20c]
[fv-az714-382:08983] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f16694ae277]
[fv-az714-382:08983] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f16694ae52b]
[fv-az714-382:08983] [ 8] plumed_master(+0x14274)[0x5612be1c6274]
[fv-az714-382:08983] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f1669029d90]
[fv-az714-382:08983] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f1669029e40]
[fv-az714-382:08983] [11] plumed_master(+0x14ed5)[0x5612be1c6ed5]
[fv-az714-382:08983] *** End of error message ***
</pre>
{% endraw %}

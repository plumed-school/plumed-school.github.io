Stderr for source:  INSTRUCTIONS.md_working_1.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:138) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[fv-az1205-759:42117] *** Process received signal ***
[fv-az1205-759:42117] Signal: Aborted (6)
[fv-az1205-759:42117] Signal code:  (-6)
[fv-az1205-759:42117] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0c1f042520]
[fv-az1205-759:42117] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0c1f0969fc]
[fv-az1205-759:42117] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0c1f042476]
[fv-az1205-759:42117] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0c1f0287f3]
[fv-az1205-759:42117] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0c1f4a2b9e]
[fv-az1205-759:42117] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0c1f4ae20c]
[fv-az1205-759:42117] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0c1f4ae277]
[fv-az1205-759:42117] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0c1f4ae52b]
[fv-az1205-759:42117] [ 8] plumed_master(+0x14274)[0x5586b416f274]
[fv-az1205-759:42117] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0c1f029d90]
[fv-az1205-759:42117] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0c1f029e40]
[fv-az1205-759:42117] [11] plumed_master(+0x14ed5)[0x5586b416fed5]
[fv-az1205-759:42117] *** End of error message ***
</pre>
{% endraw %}

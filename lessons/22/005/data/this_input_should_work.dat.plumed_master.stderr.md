Stderr for source:  this_input_should_work.dat   
Download: [zipped raw stdout](this_input_should_work.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](this_input_should_work.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:139) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[fv-az523-443:67137] *** Process received signal ***
[fv-az523-443:67137] Signal: Aborted (6)
[fv-az523-443:67137] Signal code:  (-6)
[fv-az523-443:67137] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fd2a8c42520]
[fv-az523-443:67137] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fd2a8c969fc]
[fv-az523-443:67137] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fd2a8c42476]
[fv-az523-443:67137] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fd2a8c287f3]
[fv-az523-443:67137] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7fd2a90a4f26]
[fv-az523-443:67137] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7fd2a90b6d9c]
[fv-az523-443:67137] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7fd2a90b6e07]
[fv-az523-443:67137] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fd2a90b70bb]
[fv-az523-443:67137] [ 8] plumed_master(+0x12e7f)[0x5621e1792e7f]
[fv-az523-443:67137] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fd2a8c29d90]
[fv-az523-443:67137] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fd2a8c29e40]
[fv-az523-443:67137] [11] plumed_master(+0x13115)[0x5621e1793115]
[fv-az523-443:67137] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  this_input_should_work.dat   
Download: [zipped raw stdout](this_input_should_work.dat.plumed.stdout.txt.zip) - [zipped raw stderr](this_input_should_work.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:124) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[fv-az523-443:67129] *** Process received signal ***
[fv-az523-443:67129] Signal: Aborted (6)
[fv-az523-443:67129] Signal code:  (-6)
[fv-az523-443:67129] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7feafc842520]
[fv-az523-443:67129] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7feafc8969fc]
[fv-az523-443:67129] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7feafc842476]
[fv-az523-443:67129] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7feafc8287f3]
[fv-az523-443:67129] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa4f26)[0x7feafcca4f26]
[fv-az523-443:67129] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6d9c)[0x7feafccb6d9c]
[fv-az523-443:67129] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb6e07)[0x7feafccb6e07]
[fv-az523-443:67129] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7feafccb70bb]
[fv-az523-443:67129] [ 8] plumed(+0x12f48)[0x55e568ab2f48]
[fv-az523-443:67129] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7feafc829d90]
[fv-az523-443:67129] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7feafc829e40]
[fv-az523-443:67129] [11] plumed(+0x131e5)[0x55e568ab31e5]
[fv-az523-443:67129] *** End of error message ***
</pre>
{% endraw %}

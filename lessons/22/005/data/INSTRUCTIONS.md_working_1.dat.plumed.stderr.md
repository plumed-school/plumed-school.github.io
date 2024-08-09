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
[fv-az714-382:08974] *** Process received signal ***
[fv-az714-382:08974] Signal: Aborted (6)
[fv-az714-382:08974] Signal code:  (-6)
[fv-az714-382:08974] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff0eb242520]
[fv-az714-382:08974] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff0eb2969fc]
[fv-az714-382:08974] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff0eb242476]
[fv-az714-382:08974] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff0eb2287f3]
[fv-az714-382:08974] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff0eb6a2b9e]
[fv-az714-382:08974] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff0eb6ae20c]
[fv-az714-382:08974] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff0eb6ae277]
[fv-az714-382:08974] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff0eb6ae52b]
[fv-az714-382:08974] [ 8] plumed(+0x12f48)[0x562cf39d6f48]
[fv-az714-382:08974] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff0eb229d90]
[fv-az714-382:08974] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff0eb229e40]
[fv-az714-382:08974] [11] plumed(+0x131e5)[0x562cf39d71e5]
[fv-az714-382:08974] *** End of error message ***
</pre>
{% endraw %}

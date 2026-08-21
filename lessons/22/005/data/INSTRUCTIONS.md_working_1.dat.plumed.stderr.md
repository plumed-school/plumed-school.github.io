Stderr for source:  INSTRUCTIONS.md_working_1.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(pytorch/PytorchModel.cpp:136) PLMD::function::pytorch::PytorchModel::PytorchModel(const PLMD::ActionOptions&)
The FILE: 'torch_model.ptc' does not exist.
[runnervm76f27:06170] *** Process received signal ***
[runnervm76f27:06170] Signal: Aborted (6)
[runnervm76f27:06170] Signal code:  (-6)
[runnervm76f27:06170] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa7bd445330]
[runnervm76f27:06170] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa7bd49ec0c]
[runnervm76f27:06170] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa7bd44527e]
[runnervm76f27:06170] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa7bd4288ff]
[runnervm76f27:06170] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa7bd8a5ff5]
[runnervm76f27:06170] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa7bd8bb0da]
[runnervm76f27:06170] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa7bd8a5a55]
[runnervm76f27:06170] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa7bd8a5a6f]
[runnervm76f27:06170] [ 8] plumed(+0x146dd)[0x5584de3fc6dd]
[runnervm76f27:06170] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa7bd42a1ca]
[runnervm76f27:06170] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa7bd42a28b]
[runnervm76f27:06170] [11] plumed(+0x15365)[0x5584de3fd365]
[runnervm76f27:06170] *** End of error message ***
</pre>
{% endraw %}

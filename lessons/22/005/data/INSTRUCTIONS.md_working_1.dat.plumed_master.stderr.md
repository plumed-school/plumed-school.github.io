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
[runnervm76f27:06186] *** Process received signal ***
[runnervm76f27:06186] Signal: Aborted (6)
[runnervm76f27:06186] Signal code:  (-6)
[runnervm76f27:06186] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fcbf4c45330]
[runnervm76f27:06186] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fcbf4c9ec0c]
[runnervm76f27:06186] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fcbf4c4527e]
[runnervm76f27:06186] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fcbf4c288ff]
[runnervm76f27:06186] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fcbf50a5ff5]
[runnervm76f27:06186] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fcbf50bb0da]
[runnervm76f27:06186] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fcbf50a5a55]
[runnervm76f27:06186] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fcbf50a5a6f]
[runnervm76f27:06186] [ 8] plumed_master(+0x146dd)[0x55bad0fe76dd]
[runnervm76f27:06186] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fcbf4c2a1ca]
[runnervm76f27:06186] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fcbf4c2a28b]
[runnervm76f27:06186] [11] plumed_master(+0x15365)[0x55bad0fe8365]
[runnervm76f27:06186] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  examples.md_working_1.dat   
Download: [zipped raw stdout](examples.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](examples.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/DLLoader.cpp:50) void* PLMD::DLLoader::load(const std::string&)
Could not load library /path/to/PythonCVInterface.so
/path/to/PythonCVInterface.so: cannot open shared object file: No such file or directory
[runnervm76f27:04635] *** Process received signal ***
[runnervm76f27:04635] Signal: Aborted (6)
[runnervm76f27:04635] Signal code:  (-6)
[runnervm76f27:04635] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f4f85245330]
[runnervm76f27:04635] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f4f8529ec0c]
[runnervm76f27:04635] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f4f8524527e]
[runnervm76f27:04635] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f4f852288ff]
[runnervm76f27:04635] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f4f856a5ff5]
[runnervm76f27:04635] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f4f856bb0da]
[runnervm76f27:04635] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f4f856a5a55]
[runnervm76f27:04635] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f4f856a5a6f]
[runnervm76f27:04635] [ 8] plumed(+0x146dd)[0x55dbdf97c6dd]
[runnervm76f27:04635] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f4f8522a1ca]
[runnervm76f27:04635] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f4f8522a28b]
[runnervm76f27:04635] [11] plumed(+0x15365)[0x55dbdf97d365]
[runnervm76f27:04635] *** End of error message ***
</pre>
{% endraw %}

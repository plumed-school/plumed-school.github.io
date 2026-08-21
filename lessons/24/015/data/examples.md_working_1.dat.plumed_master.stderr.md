Stderr for source:  examples.md_working_1.dat   
Download: [zipped raw stdout](examples.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](examples.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/DLLoader.cpp:50) void* PLMD::DLLoader::load(const std::string&)
Could not load library /path/to/PythonCVInterface.so
/path/to/PythonCVInterface.so: cannot open shared object file: No such file or directory
[runnervm76f27:04651] *** Process received signal ***
[runnervm76f27:04651] Signal: Aborted (6)
[runnervm76f27:04651] Signal code:  (-6)
[runnervm76f27:04651] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f3ad1845330]
[runnervm76f27:04651] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f3ad189ec0c]
[runnervm76f27:04651] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f3ad184527e]
[runnervm76f27:04651] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f3ad18288ff]
[runnervm76f27:04651] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f3ad1ca5ff5]
[runnervm76f27:04651] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f3ad1cbb0da]
[runnervm76f27:04651] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f3ad1ca5a55]
[runnervm76f27:04651] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f3ad1ca5a6f]
[runnervm76f27:04651] [ 8] plumed_master(+0x146dd)[0x555f37e586dd]
[runnervm76f27:04651] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f3ad182a1ca]
[runnervm76f27:04651] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f3ad182a28b]
[runnervm76f27:04651] [11] plumed_master(+0x15365)[0x555f37e59365]
[runnervm76f27:04651] *** End of error message ***
</pre>
{% endraw %}

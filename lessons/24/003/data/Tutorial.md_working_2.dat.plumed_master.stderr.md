Stderr for source:  Tutorial.md_working_2.dat   
Download: [zipped raw stdout](Tutorial.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](Tutorial.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/NeighborList.cpp:117) void PLMD::NeighborList::initialize()
A NeighborList is trying to allocate 39 GB of data for the list of neighbors
You can skip this error by exporting "PLUMED_IGNORE_NL_MEMORY_ERROR"
[runnervm76f27:05076] *** Process received signal ***
[runnervm76f27:05076] Signal: Aborted (6)
[runnervm76f27:05076] Signal code:  (-6)
[runnervm76f27:05076] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f6206845330]
[runnervm76f27:05076] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f620689ec0c]
[runnervm76f27:05076] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f620684527e]
[runnervm76f27:05076] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f62068288ff]
[runnervm76f27:05076] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f6206ca5ff5]
[runnervm76f27:05076] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f6206cbb0da]
[runnervm76f27:05076] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f6206ca5a55]
[runnervm76f27:05076] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f6206ca5a6f]
[runnervm76f27:05076] [ 8] plumed_master(+0x146dd)[0x55abc24e86dd]
[runnervm76f27:05076] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f620682a1ca]
[runnervm76f27:05076] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f620682a28b]
[runnervm76f27:05076] [11] plumed_master(+0x15365)[0x55abc24e9365]
[runnervm76f27:05076] *** End of error message ***
</pre>
{% endraw %}

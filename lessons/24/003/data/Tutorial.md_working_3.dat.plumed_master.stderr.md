Stderr for source:  Tutorial.md_working_3.dat   
Download: [zipped raw stdout](Tutorial.md_working_3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](Tutorial.md_working_3.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/NeighborList.cpp:117) void PLMD::NeighborList::initialize()
A NeighborList is trying to allocate 39 GB of data for the list of neighbors
You can skip this error by exporting "PLUMED_IGNORE_NL_MEMORY_ERROR"
[runnervm76f27:05121] *** Process received signal ***
[runnervm76f27:05121] Signal: Aborted (6)
[runnervm76f27:05121] Signal code:  (-6)
[runnervm76f27:05121] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fee7a245330]
[runnervm76f27:05121] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fee7a29ec0c]
[runnervm76f27:05121] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fee7a24527e]
[runnervm76f27:05121] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fee7a2288ff]
[runnervm76f27:05121] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fee7a6a5ff5]
[runnervm76f27:05121] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fee7a6bb0da]
[runnervm76f27:05121] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fee7a6a5a55]
[runnervm76f27:05121] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fee7a6a5a6f]
[runnervm76f27:05121] [ 8] plumed_master(+0x146dd)[0x55e95e43b6dd]
[runnervm76f27:05121] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fee7a22a1ca]
[runnervm76f27:05121] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fee7a22a28b]
[runnervm76f27:05121] [11] plumed_master(+0x15365)[0x55e95e43c365]
[runnervm76f27:05121] *** End of error message ***
</pre>
{% endraw %}

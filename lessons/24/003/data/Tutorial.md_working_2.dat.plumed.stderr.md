Stderr for source:  Tutorial.md_working_2.dat   
Download: [zipped raw stdout](Tutorial.md_working_2.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Tutorial.md_working_2.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(tools/NeighborList.cpp:108) void PLMD::NeighborList::initialize()
A NeighborList is trying to allocate 39 GB of data for the list of neighbors
You can skip this error by exporting "PLUMED_IGNORE_NL_MEMORY_ERROR"
[runnervm76f27:05060] *** Process received signal ***
[runnervm76f27:05060] Signal: Aborted (6)
[runnervm76f27:05060] Signal code:  (-6)
[runnervm76f27:05060] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f70bbc45330]
[runnervm76f27:05060] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f70bbc9ec0c]
[runnervm76f27:05060] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f70bbc4527e]
[runnervm76f27:05060] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f70bbc288ff]
[runnervm76f27:05060] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f70bc0a5ff5]
[runnervm76f27:05060] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f70bc0bb0da]
[runnervm76f27:05060] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f70bc0a5a55]
[runnervm76f27:05060] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f70bc0a5a6f]
[runnervm76f27:05060] [ 8] plumed(+0x146dd)[0x560cbc0ce6dd]
[runnervm76f27:05060] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f70bbc2a1ca]
[runnervm76f27:05060] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f70bbc2a28b]
[runnervm76f27:05060] [11] plumed(+0x15365)[0x560cbc0cf365]
[runnervm76f27:05060] *** End of error message ***
</pre>
{% endraw %}

Stderr for source:  Tutorial.md_working_2.dat   
Download: [zipped raw stdout](Tutorial.md_working_2.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](Tutorial.md_working_2.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():  std::bad_alloc

The above exception was the direct cause of the following exception:

(tools/NeighborList.cpp:117) void PLMD::NeighborList::initialize()
An error happened while allocating the neighbor list, please decrease the number of atoms used
[fv-az1205-759:41221] *** Process received signal ***
[fv-az1205-759:41221] Signal: Aborted (6)
[fv-az1205-759:41221] Signal code:  (-6)
[fv-az1205-759:41221] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3e81042520]
[fv-az1205-759:41221] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f3e810969fc]
[fv-az1205-759:41221] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3e81042476]
[fv-az1205-759:41221] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f3e810287f3]
[fv-az1205-759:41221] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f3e814a2b9e]
[fv-az1205-759:41221] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f3e814ae20c]
[fv-az1205-759:41221] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f3e814ae277]
[fv-az1205-759:41221] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f3e814ae52b]
[fv-az1205-759:41221] [ 8] plumed_master(+0x14274)[0x5576f44ea274]
[fv-az1205-759:41221] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3e81029d90]
[fv-az1205-759:41221] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3e81029e40]
[fv-az1205-759:41221] [11] plumed_master(+0x14ed5)[0x5576f44eaed5]
[fv-az1205-759:41221] *** End of error message ***
</pre>
{% endraw %}

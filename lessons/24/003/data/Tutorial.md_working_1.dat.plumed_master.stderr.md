Stderr for source:  Tutorial.md_working_1.dat   
Download: [zipped raw stdout](Tutorial.md_working_1.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](Tutorial.md_working_1.dat.plumed_master.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():  std::bad_alloc

The above exception was the direct cause of the following exception:

(tools/NeighborList.cpp:117) void PLMD::NeighborList::initialize()
An error happened while allocating the neighbor list, please decrease the number of atoms used
[fv-az1205-759:41189] *** Process received signal ***
[fv-az1205-759:41189] Signal: Aborted (6)
[fv-az1205-759:41189] Signal code:  (-6)
[fv-az1205-759:41189] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f11aa642520]
[fv-az1205-759:41189] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f11aa6969fc]
[fv-az1205-759:41189] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f11aa642476]
[fv-az1205-759:41189] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f11aa6287f3]
[fv-az1205-759:41189] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f11aaaa2b9e]
[fv-az1205-759:41189] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f11aaaae20c]
[fv-az1205-759:41189] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f11aaaae277]
[fv-az1205-759:41189] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f11aaaae52b]
[fv-az1205-759:41189] [ 8] plumed_master(+0x14274)[0x55f78e9c6274]
[fv-az1205-759:41189] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f11aa629d90]
[fv-az1205-759:41189] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f11aa629e40]
[fv-az1205-759:41189] [11] plumed_master(+0x14ed5)[0x55f78e9c6ed5]
[fv-az1205-759:41189] *** End of error message ***
</pre>
{% endraw %}

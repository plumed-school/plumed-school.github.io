Stderr for source:  plumed_ex1.dat   
Download: [zipped raw stdout](plumed_ex1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action METAD with label metad : action cv has no component named cv (hint! the components in this actions are: cv.x cv.y cv.z )
[runnervm76f27:05550] *** Process received signal ***
[runnervm76f27:05550] Signal: Aborted (6)
[runnervm76f27:05550] Signal code:  (-6)
[runnervm76f27:05550] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7f8289245330]
[runnervm76f27:05550] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7f828929ec0c]
[runnervm76f27:05550] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7f828924527e]
[runnervm76f27:05550] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7f82892288ff]
[runnervm76f27:05550] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7f82896a5ff5]
[runnervm76f27:05550] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7f82896bb0da]
[runnervm76f27:05550] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7f82896a5a55]
[runnervm76f27:05550] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7f82896a5a6f]
[runnervm76f27:05550] [ 8] plumed(+0x146dd)[0x5592975126dd]
[runnervm76f27:05550] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7f828922a1ca]
[runnervm76f27:05550] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7f828922a28b]
[runnervm76f27:05550] [11] plumed(+0x15365)[0x559297513365]
[runnervm76f27:05550] *** End of error message ***
</pre>
{% endraw %}

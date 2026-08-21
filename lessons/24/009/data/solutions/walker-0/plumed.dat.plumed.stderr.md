Stderr for source:  ./solutions/walker-0/plumed.dat   
Download: [zipped raw stdout](plumed.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:375) void PLMD::Action::error(const std::string&) const
ERROR in input to action HBOND_MATRIX with label hbmat1 : cannot understand the following words from the input line : SUM
[runnervm76f27:04009] *** Process received signal ***
[runnervm76f27:04009] Signal: Aborted (6)
[runnervm76f27:04009] Signal code:  (-6)
[runnervm76f27:04009] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x45330)[0x7fa602a45330]
[runnervm76f27:04009] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x11c)[0x7fa602a9ec0c]
[runnervm76f27:04009] [ 2] /lib/x86_64-linux-gnu/libc.so.6(gsignal+0x1e)[0x7fa602a4527e]
[runnervm76f27:04009] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xdf)[0x7fa602a288ff]
[runnervm76f27:04009] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5ff5)[0x7fa602ea5ff5]
[runnervm76f27:04009] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xbb0da)[0x7fa602ebb0da]
[runnervm76f27:04009] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0x0)[0x7fa602ea5a55]
[runnervm76f27:04009] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa5a6f)[0x7fa602ea5a6f]
[runnervm76f27:04009] [ 8] plumed(+0x146dd)[0x55c8813516dd]
[runnervm76f27:04009] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x2a1ca)[0x7fa602a2a1ca]
[runnervm76f27:04009] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x8b)[0x7fa602a2a28b]
[runnervm76f27:04009] [11] plumed(+0x15365)[0x55c881352365]
[runnervm76f27:04009] *** End of error message ***
</pre>
{% endraw %}

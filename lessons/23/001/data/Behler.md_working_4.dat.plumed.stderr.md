Stderr for source:  Behler.md_working_4.dat   
Download: [zipped raw stdout](Behler.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](Behler.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action DISTANCE with label d1 : Number of specified atoms should be 2
[fv-az714-382:07075] *** Process received signal ***
[fv-az714-382:07075] Signal: Aborted (6)
[fv-az714-382:07075] Signal code:  (-6)
[fv-az714-382:07075] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff73e442520]
[fv-az714-382:07075] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff73e4969fc]
[fv-az714-382:07075] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff73e442476]
[fv-az714-382:07075] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff73e4287f3]
[fv-az714-382:07075] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7ff73e8a2b9e]
[fv-az714-382:07075] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7ff73e8ae20c]
[fv-az714-382:07075] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7ff73e8ae277]
[fv-az714-382:07075] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7ff73e8ae52b]
[fv-az714-382:07075] [ 8] plumed(+0x12f48)[0x56218842ef48]
[fv-az714-382:07075] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff73e429d90]
[fv-az714-382:07075] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff73e429e40]
[fv-az714-382:07075] [11] plumed(+0x131e5)[0x56218842f1e5]
[fv-az714-382:07075] *** End of error message ***
</pre>
{% endraw %}

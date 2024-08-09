Stderr for source:  INSTRUCTIONS.md_working_7.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_7.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_7.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: )
[fv-az714-382:08785] *** Process received signal ***
[fv-az714-382:08785] Signal: Aborted (6)
[fv-az714-382:08785] Signal code:  (-6)
[fv-az714-382:08785] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f0bbb442520]
[fv-az714-382:08785] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f0bbb4969fc]
[fv-az714-382:08785] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f0bbb442476]
[fv-az714-382:08785] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f0bbb4287f3]
[fv-az714-382:08785] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7f0bbb8a2b9e]
[fv-az714-382:08785] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7f0bbb8ae20c]
[fv-az714-382:08785] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7f0bbb8ae277]
[fv-az714-382:08785] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7f0bbb8ae52b]
[fv-az714-382:08785] [ 8] plumed(+0x12f48)[0x562e6faacf48]
[fv-az714-382:08785] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f0bbb429d90]
[fv-az714-382:08785] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f0bbb429e40]
[fv-az714-382:08785] [11] plumed(+0x131e5)[0x562e6faad1e5]
[fv-az714-382:08785] *** End of error message ***
</pre>
{% endraw %}

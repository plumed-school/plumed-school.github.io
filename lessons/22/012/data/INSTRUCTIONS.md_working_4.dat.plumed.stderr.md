Stderr for source:  INSTRUCTIONS.md_working_4.dat   
Download: [zipped raw stdout](INSTRUCTIONS.md_working_4.dat.plumed.stdout.txt.zip) - [zipped raw stderr](INSTRUCTIONS.md_working_4.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/Action.cpp:240) void PLMD::Action::error(const string&) const
ERROR in input to action OPES_METAD with label opes : cannot find action named cv (hint! the actions with value in this ActionSet are: )
[fv-az714-382:08691] *** Process received signal ***
[fv-az714-382:08691] Signal: Aborted (6)
[fv-az714-382:08691] Signal code:  (-6)
[fv-az714-382:08691] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fc395842520]
[fv-az714-382:08691] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fc3958969fc]
[fv-az714-382:08691] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fc395842476]
[fv-az714-382:08691] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fc3958287f3]
[fv-az714-382:08691] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fc395ca2b9e]
[fv-az714-382:08691] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fc395cae20c]
[fv-az714-382:08691] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fc395cae277]
[fv-az714-382:08691] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fc395cae52b]
[fv-az714-382:08691] [ 8] plumed(+0x12f48)[0x5639055a0f48]
[fv-az714-382:08691] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fc395829d90]
[fv-az714-382:08691] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fc395829e40]
[fv-az714-382:08691] [11] plumed(+0x131e5)[0x5639055a11e5]
[fv-az714-382:08691] *** End of error message ***
</pre>
{% endraw %}

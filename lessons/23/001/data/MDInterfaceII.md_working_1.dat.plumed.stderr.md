Stderr for source:  MDInterfaceII.md_working_1.dat   
Download: [zipped raw stdout](MDInterfaceII.md_working_1.dat.plumed.stdout.txt.zip) - [zipped raw stderr](MDInterfaceII.md_working_1.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
terminate called after throwing an instance of 'PLMD::Plumed::ExceptionError'
what():
(core/PlumedMain.cpp:824) void PLMD::PlumedMain::readInputWords(const std::vector<std::__cxx11::basic_string<char> >&)
ERROR
I cannot understand line: DOMAIN_DECOMPOSITION LABEL=gromacs NATOMS=2000 VALUE1=myposx UNIT1=length PERIODIC1=NO CONSTANT1=False ROLE1=x VALUE2=myposy UNIT2=length PERIODIC2=NO CONSTANT2=False ROLE2=y VALUE3=myposz UNIT3=length PERIODIC3=NO CONSTANT3=False ROLE3=z VALUE4=myMasses UNIT4=mass PERIODIC4=NO CONSTANT4=True ROLE4=m VALUE5=myCharges UNIT5=charge PERIODIC5=NO CONSTANT5=True ROLE5=q PBCLABEL=mybox
Maybe a missing space or a typo?
[fv-az714-650:41214] *** Process received signal ***
[fv-az714-650:41214] Signal: Aborted (6)
[fv-az714-650:41214] Signal code:  (-6)
[fv-az714-650:41214] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa84b242520]
[fv-az714-650:41214] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa84b2969fc]
[fv-az714-650:41214] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa84b242476]
[fv-az714-650:41214] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa84b2287f3]
[fv-az714-650:41214] [ 4] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa2b9e)[0x7fa84b6a2b9e]
[fv-az714-650:41214] [ 5] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae20c)[0x7fa84b6ae20c]
[fv-az714-650:41214] [ 6] /lib/x86_64-linux-gnu/libstdc++.so.6(+0xae277)[0x7fa84b6ae277]
[fv-az714-650:41214] [ 7] /lib/x86_64-linux-gnu/libstdc++.so.6(__cxa_rethrow+0x4b)[0x7fa84b6ae52b]
[fv-az714-650:41214] [ 8] plumed(+0x12f48)[0x5586e5337f48]
[fv-az714-650:41214] [ 9] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa84b229d90]
[fv-az714-650:41214] [10] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa84b229e40]
[fv-az714-650:41214] [11] plumed(+0x131e5)[0x5586e53381e5]
[fv-az714-650:41214] *** End of error message ***
</pre>
{% endraw %}

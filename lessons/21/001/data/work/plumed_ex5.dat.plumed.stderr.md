Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed.stderr.txt.zip) 
{% raw %}
<pre>
#! Only the first 1000 rows of the error file are shown below
#! To inspect the full error file, please download the zipped raw stderr file above
A process has executed an operation involving a call
to the fork() system call to create a child process.

As a result, the libfabric EFA provider is operating in
a condition that could result in memory corruption or
other system errors.

For the libfabric EFA provider to work safely when fork()
is called, you will need to set the following environment
variable:
RDMAV_FORK_SAFE

However, setting this environment variable can result in
signficant performance impact to your application due to
increased cost of memory registration.

You may want to check with your application vendor to see
if an application-level alternative (of not using fork)
exists.

Your job will now abort.
[fv-az695-474:65134] *** Process received signal ***
[fv-az695-474:65134] Signal: Aborted (6)
[fv-az695-474:65134] Signal code:  (-6)
[fv-az695-474:65134] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff122042520]
[fv-az695-474:65134] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff1220969fc]
[fv-az695-474:65134] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff122042476]
[fv-az695-474:65134] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff1220287f3]
[fv-az695-474:65134] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7ff105121b4e]
[fv-az695-474:65134] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7ff1220eaf48]
[fv-az695-474:65134] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7ff1220ea711]
[fv-az695-474:65134] [ 7] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xbc)[0x7ff1233a25fc]
[fv-az695-474:65134] [ 8] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x163d)[0x7ff122ea337d]
[fv-az695-474:65134] [ 9] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x547)[0x7ff122e61297]
[fv-az695-474:65134] [10] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0xf1)[0x7ff122e61a41]
[fv-az695-474:65134] [11] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x23e)[0x7ff122ffee4e]
[fv-az695-474:65134] [12] /home/runner/opt/lib/libplumedKernel.so(+0x7ffe87)[0x7ff122fffe87]
[fv-az695-474:65134] [13] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7ff122e6744c]
[fv-az695-474:65134] [14] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EE+0x288)[0x7ff122eb3a18]
[fv-az695-474:65134] [15] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x54)[0x7ff122eb3eb4]
[fv-az695-474:65134] [16] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xa6)[0x7ff122eb6686]
[fv-az695-474:65134] [17] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain4initEv+0x13ba)[0x7ff122eb7c1a]
[fv-az695-474:65134] [18] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x2566)[0x7ff122eba726]
[fv-az695-474:65134] [19] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x313e)[0x7ff122c4c8fe]
[fv-az695-474:65134] [20] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7ff122e81b33]
[fv-az695-474:65134] [21] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x67e)[0x7ff122e8476e]
[fv-az695-474:65134] [22] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x208d)[0x7ff122eba24d]
[fv-az695-474:65134] [23] /home/runner/opt/lib/libplumedKernel.so(+0x6c0645)[0x7ff122ec0645]
[fv-az695-474:65134] [24] plumed(+0x1a6f0)[0x559f0fb2d6f0]
[fv-az695-474:65134] [25] plumed(+0x1364e)[0x559f0fb2664e]
[fv-az695-474:65134] [26] plumed(+0x1311c)[0x559f0fb2611c]
[fv-az695-474:65134] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff122029d90]
[fv-az695-474:65134] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff122029e40]
[fv-az695-474:65134] [29] plumed(+0x131e5)[0x559f0fb261e5]
[fv-az695-474:65134] *** End of error message ***
</pre>
{% endraw %}

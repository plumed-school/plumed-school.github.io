Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed.stderr.txt.zip) 
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
[fv-az695-474:65069] *** Process received signal ***
[fv-az695-474:65069] Signal: Aborted (6)
[fv-az695-474:65069] Signal code:  (-6)
[fv-az695-474:65069] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7ff8e2242520]
[fv-az695-474:65069] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7ff8e22969fc]
[fv-az695-474:65069] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7ff8e2242476]
[fv-az695-474:65069] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7ff8e22287f3]
[fv-az695-474:65069] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7ff8c6edcb4e]
[fv-az695-474:65069] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7ff8e22eaf48]
[fv-az695-474:65069] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7ff8e22ea711]
[fv-az695-474:65069] [ 7] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xbc)[0x7ff8e35a25fc]
[fv-az695-474:65069] [ 8] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x163d)[0x7ff8e30a337d]
[fv-az695-474:65069] [ 9] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x547)[0x7ff8e3061297]
[fv-az695-474:65069] [10] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0xf1)[0x7ff8e3061a41]
[fv-az695-474:65069] [11] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD6colvar8GyrationC1ERKNS_13ActionOptionsE+0xf1)[0x7ff8e3029dd1]
[fv-az695-474:65069] [12] /home/runner/opt/lib/libplumedKernel.so(+0x62a4d7)[0x7ff8e302a4d7]
[fv-az695-474:65069] [13] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7ff8e306744c]
[fv-az695-474:65069] [14] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EE+0x288)[0x7ff8e30b3a18]
[fv-az695-474:65069] [15] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x54)[0x7ff8e30b3eb4]
[fv-az695-474:65069] [16] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xa6)[0x7ff8e30b6686]
[fv-az695-474:65069] [17] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain4initEv+0x13ba)[0x7ff8e30b7c1a]
[fv-az695-474:65069] [18] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x2566)[0x7ff8e30ba726]
[fv-az695-474:65069] [19] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x313e)[0x7ff8e2e4c8fe]
[fv-az695-474:65069] [20] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7ff8e3081b33]
[fv-az695-474:65069] [21] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x67e)[0x7ff8e308476e]
[fv-az695-474:65069] [22] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x208d)[0x7ff8e30ba24d]
[fv-az695-474:65069] [23] /home/runner/opt/lib/libplumedKernel.so(+0x6c0645)[0x7ff8e30c0645]
[fv-az695-474:65069] [24] plumed(+0x1a6f0)[0x55efb1bf56f0]
[fv-az695-474:65069] [25] plumed(+0x1364e)[0x55efb1bee64e]
[fv-az695-474:65069] [26] plumed(+0x1311c)[0x55efb1bee11c]
[fv-az695-474:65069] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7ff8e2229d90]
[fv-az695-474:65069] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7ff8e2229e40]
[fv-az695-474:65069] [29] plumed(+0x131e5)[0x55efb1bee1e5]
[fv-az695-474:65069] *** End of error message ***
</pre>
{% endraw %}

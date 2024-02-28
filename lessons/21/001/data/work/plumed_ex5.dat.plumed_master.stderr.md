Stderr for source:  work/plumed_ex5.dat   
Download: [zipped raw stdout](plumed_ex5.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex5.dat.plumed_master.stderr.txt.zip) 
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
[fv-az695-474:65142] *** Process received signal ***
[fv-az695-474:65142] Signal: Aborted (6)
[fv-az695-474:65142] Signal code:  (-6)
[fv-az695-474:65142] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f869e442520]
[fv-az695-474:65142] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f869e4969fc]
[fv-az695-474:65142] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f869e442476]
[fv-az695-474:65142] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f869e4287f3]
[fv-az695-474:65142] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f8681521b4e]
[fv-az695-474:65142] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f869e4eaf48]
[fv-az695-474:65142] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f869e4ea711]
[fv-az695-474:65142] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7f869f8a55c1]
[fv-az695-474:65142] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x15d5)[0x7f869f375e65]
[fv-az695-474:65142] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x587)[0x7f869f311e17]
[fv-az695-474:65142] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x100)[0x7f869f314ff0]
[fv-az695-474:65142] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x251)[0x7f869f4cf331]
[fv-az695-474:65142] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_7generic14WholeMoleculesEE6createERKNS_13ActionOptionsE+0x27)[0x7f869f4d19e7]
[fv-az695-474:65142] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7f869f31bb5c]
[fv-az695-474:65142] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2c8)[0x7f869f380ed8]
[fv-az695-474:65142] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7f869f38139c]
[fv-az695-474:65142] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7f869f383ecf]
[fv-az695-474:65142] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xae2)[0x7f869f384a22]
[fv-az695-474:65142] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x1dc2)[0x7f869f386df2]
[fv-az695-474:65142] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2a91)[0x7f869f0ebe71]
[fv-az695-474:65142] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7f869f346cf3]
[fv-az695-474:65142] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7f869f3497de]
[fv-az695-474:65142] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x130e)[0x7f869f38633e]
[fv-az695-474:65142] [23] /home/runner/opt/lib/libplumed_masterKernel.so(+0x790b81)[0x7f869f390b81]
[fv-az695-474:65142] [24] plumed_master(+0x1acf8)[0x55c29eeebcf8]
[fv-az695-474:65142] [25] plumed_master(+0x1365e)[0x55c29eee465e]
[fv-az695-474:65142] [26] plumed_master(+0x1304c)[0x55c29eee404c]
[fv-az695-474:65142] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f869e429d90]
[fv-az695-474:65142] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f869e429e40]
[fv-az695-474:65142] [29] plumed_master(+0x13115)[0x55c29eee4115]
[fv-az695-474:65142] *** End of error message ***
</pre>
{% endraw %}

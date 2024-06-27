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
[fv-az1536-472:40043] *** Process received signal ***
[fv-az1536-472:40043] Signal: Aborted (6)
[fv-az1536-472:40043] Signal code:  (-6)
[fv-az1536-472:40043] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f7bad842520]
[fv-az1536-472:40043] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f7bad8969fc]
[fv-az1536-472:40043] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f7bad842476]
[fv-az1536-472:40043] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f7bad8287f3]
[fv-az1536-472:40043] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f7b92921b4e]
[fv-az1536-472:40043] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f7bad8eaf48]
[fv-az1536-472:40043] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f7bad8ea711]
[fv-az1536-472:40043] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7f7baef5da21]
[fv-az1536-472:40043] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x162b)[0x7f7bae8434fb]
[fv-az1536-472:40043] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKS1_IPNS_5ValueESaISC_EEPNS_6ActionERS1_INS_10AtomNumberESaISJ_EE+0x6c1)[0x7f7bae7cbc11]
[fv-az1536-472:40043] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x10d)[0x7f7bae7cd18d]
[fv-az1536-472:40043] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x251)[0x7f7baea45ef1]
[fv-az1536-472:40043] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_7generic14WholeMoleculesEE6createERKNS_13ActionOptionsE+0x27)[0x7f7baea48597]
[fv-az1536-472:40043] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKSt6vectorIPvSaIS2_EERKNS_13ActionOptionsE+0x383)[0x7f7bae7d03f3]
[fv-az1536-472:40043] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2da)[0x7f7bae856a8a]
[fv-az1536-472:40043] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7f7bae85723c]
[fv-az1536-472:40043] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7f7bae85c94f]
[fv-az1536-472:40043] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xb6a)[0x7f7bae85d52a]
[fv-az1536-472:40043] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x29bf)[0x7f7bae8604cf]
[fv-az1536-472:40043] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2b2a)[0x7f7bae54d90a]
[fv-az1536-472:40043] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d2)[0x7f7bae812992]
[fv-az1536-472:40043] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7f7bae8153fe]
[fv-az1536-472:40043] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x12d4)[0x7f7bae85ede4]
[fv-az1536-472:40043] [23] /home/runner/opt/lib/libplumed_masterKernel.so(+0x8684c1)[0x7f7bae8684c1]
[fv-az1536-472:40043] [24] plumed_master(+0x1e207)[0x55d0f1085207]
[fv-az1536-472:40043] [25] plumed_master(+0x14d61)[0x55d0f107bd61]
[fv-az1536-472:40043] [26] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f7bad829d90]
[fv-az1536-472:40043] [27] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f7bad829e40]
[fv-az1536-472:40043] [28] plumed_master(+0x14ed5)[0x55d0f107bed5]
[fv-az1536-472:40043] *** End of error message ***
</pre>
{% endraw %}

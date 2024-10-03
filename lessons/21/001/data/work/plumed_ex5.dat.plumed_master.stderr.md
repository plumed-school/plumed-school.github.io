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
[fv-az740-873:42833] *** Process received signal ***
[fv-az740-873:42833] Signal: Aborted (6)
[fv-az740-873:42833] Signal code:  (-6)
[fv-az740-873:42833] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f93ada42520]
[fv-az740-873:42833] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f93ada969fc]
[fv-az740-873:42833] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f93ada42476]
[fv-az740-873:42833] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f93ada287f3]
[fv-az740-873:42833] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f9393f21b4e]
[fv-az740-873:42833] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f93adaeaf48]
[fv-az740-873:42833] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f93adaea711]
[fv-az740-873:42833] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7f93af185301]
[fv-az740-873:42833] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x162b)[0x7f93aea556bb]
[fv-az740-873:42833] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKS1_IPNS_5ValueESaISC_EEPNS_6ActionERS1_INS_10AtomNumberESaISJ_EE+0x6c1)[0x7f93ae9dc941]
[fv-az740-873:42833] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x10d)[0x7f93ae9ddebd]
[fv-az740-873:42833] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x251)[0x7f93aec63ba1]
[fv-az740-873:42833] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_7generic14WholeMoleculesEE6createERKNS_13ActionOptionsE+0x27)[0x7f93aec66247]
[fv-az740-873:42833] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKSt6vectorIPvSaIS2_EERKNS_13ActionOptionsE+0x3f9)[0x7f93ae9e12e9]
[fv-az740-873:42833] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2da)[0x7f93aea68caa]
[fv-az740-873:42833] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7f93aea6945c]
[fv-az740-873:42833] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7f93aea6eb6f]
[fv-az740-873:42833] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xb6a)[0x7f93aea6f74a]
[fv-az740-873:42833] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x29bf)[0x7f93aea726ef]
[fv-az740-873:42833] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2b2a)[0x7f93ae75680a]
[fv-az740-873:42833] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d2)[0x7f93aea24782]
[fv-az740-873:42833] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7f93aea271ee]
[fv-az740-873:42833] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x12d4)[0x7f93aea71004]
[fv-az740-873:42833] [23] /home/runner/opt/lib/libplumed_masterKernel.so(+0x87a6e1)[0x7f93aea7a6e1]
[fv-az740-873:42833] [24] plumed_master(+0x1e207)[0x5639fb4f9207]
[fv-az740-873:42833] [25] plumed_master(+0x14d61)[0x5639fb4efd61]
[fv-az740-873:42833] [26] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f93ada29d90]
[fv-az740-873:42833] [27] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f93ada29e40]
[fv-az740-873:42833] [28] plumed_master(+0x14ed5)[0x5639fb4efed5]
[fv-az740-873:42833] *** End of error message ***
</pre>
{% endraw %}

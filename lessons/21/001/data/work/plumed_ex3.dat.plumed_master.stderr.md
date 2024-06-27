Stderr for source:  work/plumed_ex3.dat   
Download: [zipped raw stdout](plumed_ex3.dat.plumed_master.stdout.txt.zip) - [zipped raw stderr](plumed_ex3.dat.plumed_master.stderr.txt.zip) 
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
[fv-az1536-472:39982] *** Process received signal ***
[fv-az1536-472:39982] Signal: Aborted (6)
[fv-az1536-472:39982] Signal code:  (-6)
[fv-az1536-472:39982] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f8e9bc42520]
[fv-az1536-472:39982] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f8e9bc969fc]
[fv-az1536-472:39982] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f8e9bc42476]
[fv-az1536-472:39982] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f8e9bc287f3]
[fv-az1536-472:39982] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f8e84944b4e]
[fv-az1536-472:39982] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f8e9bceaf48]
[fv-az1536-472:39982] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f8e9bcea711]
[fv-az1536-472:39982] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7f8e9d35da21]
[fv-az1536-472:39982] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x162b)[0x7f8e9cc434fb]
[fv-az1536-472:39982] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKS1_IPNS_5ValueESaISC_EEPNS_6ActionERS1_INS_10AtomNumberESaISJ_EE+0x6c1)[0x7f8e9cbcbc11]
[fv-az1536-472:39982] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x10d)[0x7f8e9cbcd18d]
[fv-az1536-472:39982] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD6colvar8GyrationC1ERKNS_13ActionOptionsE+0x103)[0x7f8e9cb370e3]
[fv-az1536-472:39982] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_6colvar8GyrationEE6createERKNS_13ActionOptionsE+0x27)[0x7f8e9cb39b57]
[fv-az1536-472:39982] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKSt6vectorIPvSaIS2_EERKNS_13ActionOptionsE+0x383)[0x7f8e9cbd03f3]
[fv-az1536-472:39982] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2da)[0x7f8e9cc56a8a]
[fv-az1536-472:39982] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputLineERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKb+0xba)[0x7f8e9cc56e4a]
[fv-az1536-472:39982] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionShortcut13readInputLineERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEb+0x2cf)[0x7f8e9cbdbdef]
[fv-az1536-472:39982] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD6colvar16GyrationShortcutC1ERKNS_13ActionOptionsE+0x539)[0x7f8e9cb3fbd9]
[fv-az1536-472:39982] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_6colvar16GyrationShortcutEE6createERKNS_13ActionOptionsE+0x27)[0x7f8e9cb44427]
[fv-az1536-472:39982] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKSt6vectorIPvSaIS2_EERKNS_13ActionOptionsE+0x383)[0x7f8e9cbd03f3]
[fv-az1536-472:39982] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2da)[0x7f8e9cc56a8a]
[fv-az1536-472:39982] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7f8e9cc5723c]
[fv-az1536-472:39982] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7f8e9cc5c94f]
[fv-az1536-472:39982] [23] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xb6a)[0x7f8e9cc5d52a]
[fv-az1536-472:39982] [24] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x29bf)[0x7f8e9cc604cf]
[fv-az1536-472:39982] [25] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2b2a)[0x7f8e9c94d90a]
[fv-az1536-472:39982] [26] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d2)[0x7f8e9cc12992]
[fv-az1536-472:39982] [27] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7f8e9cc153fe]
[fv-az1536-472:39982] [28] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x12d4)[0x7f8e9cc5ede4]
[fv-az1536-472:39982] [29] /home/runner/opt/lib/libplumed_masterKernel.so(+0x8684c1)[0x7f8e9cc684c1]
[fv-az1536-472:39982] *** End of error message ***
</pre>
{% endraw %}

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
[fv-az915-95:06086] *** Process received signal ***
[fv-az915-95:06086] Signal: Aborted (6)
[fv-az915-95:06086] Signal code:  (-6)
[fv-az915-95:06086] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fda72642520]
[fv-az915-95:06086] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fda726969fc]
[fv-az915-95:06086] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fda72642476]
[fv-az915-95:06086] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fda726287f3]
[fv-az915-95:06086] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7fda55521b4e]
[fv-az915-95:06086] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7fda726eaf48]
[fv-az915-95:06086] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7fda726ea711]
[fv-az915-95:06086] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7fda73d60351]
[fv-az915-95:06086] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x162b)[0x7fda73644d5b]
[fv-az915-95:06086] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKS1_IPNS_5ValueESaISC_EEPNS_6ActionERS1_INS_10AtomNumberESaISJ_EE+0x6c1)[0x7fda735cd351]
[fv-az915-95:06086] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x10d)[0x7fda735ce8cd]
[fv-az915-95:06086] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x251)[0x7fda73847ea1]
[fv-az915-95:06086] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_7generic14WholeMoleculesEE6createERKNS_13ActionOptionsE+0x27)[0x7fda7384a547]
[fv-az915-95:06086] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKSt6vectorIPvSaIS2_EERKNS_13ActionOptionsE+0x383)[0x7fda735d1b33]
[fv-az915-95:06086] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2da)[0x7fda736582ea]
[fv-az915-95:06086] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7fda73658a9c]
[fv-az915-95:06086] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7fda7365e1af]
[fv-az915-95:06086] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xb6a)[0x7fda7365ed8a]
[fv-az915-95:06086] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x29bf)[0x7fda73661d2f]
[fv-az915-95:06086] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2b2a)[0x7fda7334e87a]
[fv-az915-95:06086] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d2)[0x7fda736141f2]
[fv-az915-95:06086] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7fda73616c5e]
[fv-az915-95:06086] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x12d4)[0x7fda73660644]
[fv-az915-95:06086] [23] /home/runner/opt/lib/libplumed_masterKernel.so(+0x869d21)[0x7fda73669d21]
[fv-az915-95:06086] [24] plumed_master(+0x1e207)[0x55e3a2e41207]
[fv-az915-95:06086] [25] plumed_master(+0x14d61)[0x55e3a2e37d61]
[fv-az915-95:06086] [26] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fda72629d90]
[fv-az915-95:06086] [27] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fda72629e40]
[fv-az915-95:06086] [28] plumed_master(+0x14ed5)[0x55e3a2e37ed5]
[fv-az915-95:06086] *** End of error message ***
</pre>
{% endraw %}

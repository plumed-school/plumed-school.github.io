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
[fv-az1536-472:40035] *** Process received signal ***
[fv-az1536-472:40035] Signal: Aborted (6)
[fv-az1536-472:40035] Signal code:  (-6)
[fv-az1536-472:40035] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f3045642520]
[fv-az1536-472:40035] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f30456969fc]
[fv-az1536-472:40035] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f3045642476]
[fv-az1536-472:40035] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f30456287f3]
[fv-az1536-472:40035] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f302a321b4e]
[fv-az1536-472:40035] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f30456eaf48]
[fv-az1536-472:40035] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f30456ea711]
[fv-az1536-472:40035] [ 7] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xbc)[0x7f30469a4ebc]
[fv-az1536-472:40035] [ 8] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x163c)[0x7f304649d68c]
[fv-az1536-472:40035] [ 9] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x547)[0x7f304645ad27]
[fv-az1536-472:40035] [10] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0xf1)[0x7f304645b4d1]
[fv-az1536-472:40035] [11] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7generic14WholeMoleculesC1ERKNS_13ActionOptionsE+0x23e)[0x7f304660157e]
[fv-az1536-472:40035] [12] /home/runner/opt/lib/libplumedKernel.so(+0x8025b7)[0x7f30466025b7]
[fv-az1536-472:40035] [13] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7f3046460edc]
[fv-az1536-472:40035] [14] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EE+0x288)[0x7f30464b6008]
[fv-az1536-472:40035] [15] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x54)[0x7f30464b64a4]
[fv-az1536-472:40035] [16] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xa6)[0x7f30464b8c76]
[fv-az1536-472:40035] [17] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain4initEv+0x13ba)[0x7f30464ba20a]
[fv-az1536-472:40035] [18] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x2566)[0x7f30464bcd16]
[fv-az1536-472:40035] [19] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x314e)[0x7f3046245fae]
[fv-az1536-472:40035] [20] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7f304647b813]
[fv-az1536-472:40035] [21] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x67e)[0x7f304647e44e]
[fv-az1536-472:40035] [22] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x208d)[0x7f30464bc83d]
[fv-az1536-472:40035] [23] /home/runner/opt/lib/libplumedKernel.so(+0x6c2d75)[0x7f30464c2d75]
[fv-az1536-472:40035] [24] plumed(+0x1a6f0)[0x56553c9d76f0]
[fv-az1536-472:40035] [25] plumed(+0x1364e)[0x56553c9d064e]
[fv-az1536-472:40035] [26] plumed(+0x1311c)[0x56553c9d011c]
[fv-az1536-472:40035] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f3045629d90]
[fv-az1536-472:40035] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f3045629e40]
[fv-az1536-472:40035] [29] plumed(+0x131e5)[0x56553c9d01e5]
[fv-az1536-472:40035] *** End of error message ***
</pre>
{% endraw %}

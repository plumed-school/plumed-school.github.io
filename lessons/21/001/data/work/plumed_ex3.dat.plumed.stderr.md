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
[fv-az1536-472:39974] *** Process received signal ***
[fv-az1536-472:39974] Signal: Aborted (6)
[fv-az1536-472:39974] Signal code:  (-6)
[fv-az1536-472:39974] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f5d27c42520]
[fv-az1536-472:39974] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f5d27c969fc]
[fv-az1536-472:39974] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f5d27c42476]
[fv-az1536-472:39974] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f5d27c287f3]
[fv-az1536-472:39974] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f5d10944b4e]
[fv-az1536-472:39974] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f5d27ceaf48]
[fv-az1536-472:39974] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f5d27cea711]
[fv-az1536-472:39974] [ 7] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xbc)[0x7f5d28fa4ebc]
[fv-az1536-472:39974] [ 8] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x163c)[0x7f5d28a9d68c]
[fv-az1536-472:39974] [ 9] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x547)[0x7f5d28a5ad27]
[fv-az1536-472:39974] [10] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0xf1)[0x7f5d28a5b4d1]
[fv-az1536-472:39974] [11] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD6colvar8GyrationC1ERKNS_13ActionOptionsE+0xf1)[0x7f5d28a23871]
[fv-az1536-472:39974] [12] /home/runner/opt/lib/libplumedKernel.so(+0x623f77)[0x7f5d28a23f77]
[fv-az1536-472:39974] [13] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7f5d28a60edc]
[fv-az1536-472:39974] [14] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EE+0x288)[0x7f5d28ab6008]
[fv-az1536-472:39974] [15] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x54)[0x7f5d28ab64a4]
[fv-az1536-472:39974] [16] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xa6)[0x7f5d28ab8c76]
[fv-az1536-472:39974] [17] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain4initEv+0x13ba)[0x7f5d28aba20a]
[fv-az1536-472:39974] [18] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x2566)[0x7f5d28abcd16]
[fv-az1536-472:39974] [19] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x314e)[0x7f5d28845fae]
[fv-az1536-472:39974] [20] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7f5d28a7b813]
[fv-az1536-472:39974] [21] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x67e)[0x7f5d28a7e44e]
[fv-az1536-472:39974] [22] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x208d)[0x7f5d28abc83d]
[fv-az1536-472:39974] [23] /home/runner/opt/lib/libplumedKernel.so(+0x6c2d75)[0x7f5d28ac2d75]
[fv-az1536-472:39974] [24] plumed(+0x1a6f0)[0x55ecc1a796f0]
[fv-az1536-472:39974] [25] plumed(+0x1364e)[0x55ecc1a7264e]
[fv-az1536-472:39974] [26] plumed(+0x1311c)[0x55ecc1a7211c]
[fv-az1536-472:39974] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f5d27c29d90]
[fv-az1536-472:39974] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f5d27c29e40]
[fv-az1536-472:39974] [29] plumed(+0x131e5)[0x55ecc1a721e5]
[fv-az1536-472:39974] *** End of error message ***
</pre>
{% endraw %}

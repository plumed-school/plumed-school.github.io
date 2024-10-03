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
[fv-az740-873:42764] *** Process received signal ***
[fv-az740-873:42764] Signal: Aborted (6)
[fv-az740-873:42764] Signal code:  (-6)
[fv-az740-873:42764] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7f9e59442520]
[fv-az740-873:42764] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7f9e594969fc]
[fv-az740-873:42764] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7f9e59442476]
[fv-az740-873:42764] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7f9e594287f3]
[fv-az740-873:42764] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7f9e3f921b4e]
[fv-az740-873:42764] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7f9e594eaf48]
[fv-az740-873:42764] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7f9e594ea711]
[fv-az740-873:42764] [ 7] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xbc)[0x7f9e5a7a4f5c]
[fv-az740-873:42764] [ 8] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x163c)[0x7f9e5a29d71c]
[fv-az740-873:42764] [ 9] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x547)[0x7f9e5a25adb7]
[fv-az740-873:42764] [10] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0xf1)[0x7f9e5a25b561]
[fv-az740-873:42764] [11] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD6colvar8GyrationC1ERKNS_13ActionOptionsE+0xf1)[0x7f9e5a223901]
[fv-az740-873:42764] [12] /home/runner/opt/lib/libplumedKernel.so(+0x624007)[0x7f9e5a224007]
[fv-az740-873:42764] [13] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7f9e5a260f6c]
[fv-az740-873:42764] [14] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EE+0x288)[0x7f9e5a2b6098]
[fv-az740-873:42764] [15] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x54)[0x7f9e5a2b6534]
[fv-az740-873:42764] [16] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xa6)[0x7f9e5a2b8d06]
[fv-az740-873:42764] [17] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain4initEv+0x13ba)[0x7f9e5a2ba29a]
[fv-az740-873:42764] [18] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x2566)[0x7f9e5a2bcda6]
[fv-az740-873:42764] [19] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x314e)[0x7f9e5a045fae]
[fv-az740-873:42764] [20] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7f9e5a27b8a3]
[fv-az740-873:42764] [21] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10CLToolMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x67e)[0x7f9e5a27e4de]
[fv-az740-873:42764] [22] /home/runner/opt/lib/libplumedKernel.so(_ZN4PLMD10PlumedMain3cmdERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERKNS_11TypesafePtrE+0x208d)[0x7f9e5a2bc8cd]
[fv-az740-873:42764] [23] /home/runner/opt/lib/libplumedKernel.so(+0x6c2e05)[0x7f9e5a2c2e05]
[fv-az740-873:42764] [24] plumed(+0x1a6f0)[0x56107b6e86f0]
[fv-az740-873:42764] [25] plumed(+0x1364e)[0x56107b6e164e]
[fv-az740-873:42764] [26] plumed(+0x1311c)[0x56107b6e111c]
[fv-az740-873:42764] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7f9e59429d90]
[fv-az740-873:42764] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7f9e59429e40]
[fv-az740-873:42764] [29] plumed(+0x131e5)[0x56107b6e11e5]
[fv-az740-873:42764] *** End of error message ***
</pre>
{% endraw %}

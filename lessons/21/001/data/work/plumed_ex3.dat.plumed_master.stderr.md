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
[fv-az695-474:65077] *** Process received signal ***
[fv-az695-474:65077] Signal: Aborted (6)
[fv-az695-474:65077] Signal code:  (-6)
[fv-az695-474:65077] [ 0] /lib/x86_64-linux-gnu/libc.so.6(+0x42520)[0x7fa2c0c42520]
[fv-az695-474:65077] [ 1] /lib/x86_64-linux-gnu/libc.so.6(pthread_kill+0x12c)[0x7fa2c0c969fc]
[fv-az695-474:65077] [ 2] /lib/x86_64-linux-gnu/libc.so.6(raise+0x16)[0x7fa2c0c42476]
[fv-az695-474:65077] [ 3] /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3)[0x7fa2c0c287f3]
[fv-az695-474:65077] [ 4] /lib/x86_64-linux-gnu/libfabric.so.1(+0x76b4e)[0x7fa2a595cb4e]
[fv-az695-474:65077] [ 5] /lib/x86_64-linux-gnu/libc.so.6(+0xeaf48)[0x7fa2c0ceaf48]
[fv-az695-474:65077] [ 6] /lib/x86_64-linux-gnu/libc.so.6(__libc_fork+0x71)[0x7fa2c0cea711]
[fv-az695-474:65077] [ 7] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10SubprocessC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0xc1)[0x7fa2c20a55c1]
[fv-az695-474:65077] [ 8] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14GenericMolInfo15interpretSymbolERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt6vectorINS_10AtomNumberESaISA_EE+0x15d5)[0x7fa2c1b75e65]
[fv-az695-474:65077] [ 9] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic17interpretAtomListERSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERS1_INS_10AtomNumberESaISB_EE+0x587)[0x7fa2c1b11e17]
[fv-az695-474:65077] [10] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD15ActionAtomistic13parseAtomListERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEiRSt6vectorINS_10AtomNumberESaISA_EE+0x100)[0x7fa2c1b14ff0]
[fv-az695-474:65077] [11] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD6colvar8GyrationC1ERKNS_13ActionOptionsE+0x103)[0x7fa2c1ad59c3]
[fv-az695-474:65077] [12] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD18ActionRegistrationINS_6colvar8GyrationEE6createERKNS_13ActionOptionsE+0x27)[0x7fa2c1ad83d7]
[fv-az695-474:65077] [13] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD14ActionRegister6createERKNS_13ActionOptionsE+0x5fc)[0x7fa2c1b1bb5c]
[fv-az695-474:65077] [14] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain14readInputWordsERKSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS7_EERKb+0x2c8)[0x7fa2c1b80ed8]
[fv-az695-474:65077] [15] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERNS_5IFileE+0x5c)[0x7fa2c1b8139c]
[fv-az695-474:65077] [16] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain13readInputFileERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE+0x9f)[0x7fa2c1b83ecf]
[fv-az695-474:65077] [17] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain4initEv+0xae2)[0x7fa2c1b84a22]
[fv-az695-474:65077] [18] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x1dc2)[0x7fa2c1b86df2]
[fv-az695-474:65077] [19] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD7cltools6DriverIdE4mainEP8_IO_FILES4_RNS_12CommunicatorE+0x2a91)[0x7fa2c18ebe71]
[fv-az695-474:65077] [20] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3runEiPPcP8_IO_FILES4_RNS_12CommunicatorE+0x7d3)[0x7fa2c1b46cf3]
[fv-az695-474:65077] [21] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10CLToolMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x53e)[0x7fa2c1b497de]
[fv-az695-474:65077] [22] /home/runner/opt/lib/libplumed_masterKernel.so(_ZN4PLMD10PlumedMain3cmdESt17basic_string_viewIcSt11char_traitsIcEERKNS_11TypesafePtrE+0x130e)[0x7fa2c1b8633e]
[fv-az695-474:65077] [23] /home/runner/opt/lib/libplumed_masterKernel.so(+0x790b81)[0x7fa2c1b90b81]
[fv-az695-474:65077] [24] plumed_master(+0x1acf8)[0x55d2d1b4acf8]
[fv-az695-474:65077] [25] plumed_master(+0x1365e)[0x55d2d1b4365e]
[fv-az695-474:65077] [26] plumed_master(+0x1304c)[0x55d2d1b4304c]
[fv-az695-474:65077] [27] /lib/x86_64-linux-gnu/libc.so.6(+0x29d90)[0x7fa2c0c29d90]
[fv-az695-474:65077] [28] /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x80)[0x7fa2c0c29e40]
[fv-az695-474:65077] [29] plumed_master(+0x13115)[0x55d2d1b43115]
[fv-az695-474:65077] *** End of error message ***
</pre>
{% endraw %}

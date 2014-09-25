mptcp-galaxy-nexsus
===================

MultipathTCP kernel port for Galaxy Nexus (maguro). 

<h3>Based on:</h3>

This is a merge of the original tuna kernel for Galaxy Nexus devices and the MPTCP kernel. It may contain bugs.

* Original kernel for Galaxy Nexus: https://android.googlesource.com/kernel/omap.git

* MultiPath TCP port to Linux Kernel v3.0: https://github.com/multipath-tcp/mptcp_3.0.x

<h3>Build:</h3>

How to build a kernel: https://source.android.com/source/building-kernels.html

* <code>make tuna_defconfig</code>
* <code>make -j 2</code>

<h3>Flash:</h3>

Be sure that you know what you are doing. This may break your device!

* <code>adb reboot bootloader</code>
* <code>fastboot flash zimage /arch/arm/boot/zImage</code>

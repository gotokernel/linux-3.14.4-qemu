The Gotokernel Open Source Project
================================================================================

Download Linux Kernel
--------------------------------------------------------------------------------

Latest Stable Kernel: linux-2.6.37.4.tar.bz2 from Linux Kernel Main Page.
Trace the source code:

```
   $ git clone git://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux-2.6.git
```

Cross Compile Linux Kernel
--------------------------------------------------------------------------------

```
   $ make ARCH=arm CROSS_COMPILE=arm-none-linux-gnueabi- versatile_defconfig -s
   $ make ARCH=arm CROSS_COMPILE=arm-none-linux-gnueabi- uImage -s
```

Then we will get the file "uImage" at the location "arch/arm/boot/".
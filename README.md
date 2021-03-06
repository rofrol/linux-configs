- https://wiki.archlinux.org/index.php/Kernels/Traditional_compilation
- https://wiki.gentoo.org/wiki/Complete_Handbook/Building_the_Linux_kernel
- http://www.linuxfromscratch.org/clfs/view/svn/x86_64-64/boot/kernel.html
- https://debian-handbook.info/browse/stable/sect.kernel-compilation.html
- https://help.ubuntu.com/community/Kernel/Compile

## localmodconfig

> `make localmodconfig` command will create a .config file for the custom kernel by disabling any and all options not currently in use by the running kernel at the time
> https://wiki.archlinux.org/index.php/Kernels/Traditional_compilation

## grep config of running kernel

```
CONFIG_IKCONFIG=y
CONFIG_IKCONFIG_PROC=y
```

http://www.linuxquestions.org/questions/linux-newbie-8/gentoo-reset-menuconfig-to-defaults-696219/#post3403200

## oldconfig

```
yes "" | make oldconfig
```

http://serverfault.com/questions/116299/automatically-answer-defaults-when-doing-make-oldconfig-on-a-kernel-tree

## 64bit

http://unix.stackexchange.com/questions/41446/how-do-i-convert-a-kernel-config-file-from-32-bit-to-64-bit

## make install and 64bit

No need to worry about copying wrong arch. x86_64 is a symlink to x86 version.

```
ls -l arch/x86_64/boot/bzImage
lrwxrwxrwx 1 root root 22 Sep  5 01:22 arch/x86_64/boot/bzImage -> ../../x86/boot/bzImage
```

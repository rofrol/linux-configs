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

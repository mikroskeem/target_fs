RPi initramfs [WIP]
=============
Features:
- Cross-compiled Linux From Scratch with musl libc

How to use:
- Download kernel source
- Unpack and do git clone https://github.com/mikroskeem/target_fs
- Put those lines to your kernel config:
```
CONFIG_BLK_DEV_INITRD=y
CONFIG_INITRAMFS_SOURCE="../target_fs"
```
- Compile kernel
- Copy arch/arm/boot/zImage to /boot/kernel.img
- Blow your Pi (It's WIP, remember?)

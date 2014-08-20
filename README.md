RPi initramfs [WIP]
=============

How to use:
- Download kernel source
- Unpack and do git clone https://github.com/mikroskeem/target_fs
- Put those lines to your kernel config:
```
CONFIG_BLK_DEV_INITRD=y
CONFIG_INITRAMFS_SOURCE="../target_fs"
```
- Run make ARCH=arm CROSS_COMPILE=/path/to/cross/compiler
- Copy arch/arm/boot/zImage to /boot/kernel.img
- Blow your Pi (It's WIP, remember?)

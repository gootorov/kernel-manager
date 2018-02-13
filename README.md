Kernel manager
===========

Simple tool to automate updating or rebuilding the kernel on Gentoo systems.

## Installation

Add my [Portage overlay](https://github.com/gootorov/gootorov-overlay) and install the package:

```Sh
# emerge sys-kernel/kernel-manager::gootorov
```

All dependencies will be pulled in automatically.

## Usage

To update the kernel to the newest version execute:

```Sh
# kernel-manager --upgrade
```
You will be asked to enable or disable the newly available options in the kernel.

To make changes to the current kernel configuration execute:

```Sh
# kernel-manager --rebuild
```
You will be prompted with the `make menuconfig` interface.

If you made changes to your initramfs or installed out-of-tree kernel modules execute:

```Sh
# kernel-manager --rebuild-initramfs
```

## Todo
- [ ] Add more flexibility
- [ ] Add a configuration file

# Linux-NSPA:

![My Image](/images/linux-nspa-banner.png)

### Linux-NSPA Archlinux Packages

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google, KernelToast, Mainline/Upstream and various other sources.

### Features/Patchwork:

* PREEMPT_RT_FULL : Realtime Linux Patchset
* Fair/RT Scheduler optimizations, modifications + backports
* Locking backport and modifications
* MM Multi-Gnerational LRU (https://lwn.net/Articles/856931/)
* MM Maple-Tree patchwork 
* Tunable WorkingSet Protection Mechanism 
* Subset of Intel Clear Linux Kernel patches
* Various Performance / interactivity related changes
* Wine-related performance patchwork
* Power management improvements
* Numerous subsystem backports from mainline, -next and tip
* Subset KernelToast's kernel patchwork
* Misc fixes/changes

SPECIAL NOTE:

The pkgbuild by default will use a kernel config for my Microsoft Surface 7.
This can be overriden and the generic kernel config can be used instead, but
that means that all modules will be build, increasing compile time 
significantly.

A generic config can be used by (un-)setting (in PKGUBILD):

_config_Surface7=

Ideally though, you will want to use your own localmodconfig via:

https://wiki.archlinux.org/title/Modprobed-db


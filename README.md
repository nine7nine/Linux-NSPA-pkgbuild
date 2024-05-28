# Linux-NSPA:

![My Image](/images/linux-nspa-banner.png)

### Linux-NSPA Archlinux Packages

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google, KernelToast, Mainline/Upstream and various other sources.

### Features/Patchwork:

* PREEMPT_RT_FULL : Realtime Linux Patchset
* Scheduler backports, optimizations, modifications, etc.
* Locking backports, hacks && modifications
* Tunable WorkingSet Protection Mechanism 
* Subset of Intel Clear Linux Kernel patches
* Subset of KernelToast's kernel patchwork
* Various Performance / interactivity related changes
* Wine-related performance patchwork
* Linux-Surface Patchwork (Microsoft Surface Devices)
* Subsystem backports from mainline & -tip
* Misc fixups, hacks and tweaks

Non-exhuastive feature list, because it tends to shift and change over-time.
Generally, I follow linux-rt-devel RT versions, but also try to follow mainline. 
It's not uncommon that I rebase an RT patch (when trivial) and/or jump to using 
mainline linux -RC kernels. However, it depends on how significant kernel changes 
are VS. my patchwork...

SPECIAL NOTE:

The pkgbuild by default will use a kernel config for my Microsoft Surface 7.
This can be overridden and the generic kernel config can be used instead, but
that means that all modules will be build, increasing compile time 
significantly.

A generic config can be used by (un-)setting (in PKGUBILD):

_config_Surface7=

Ideally though, you will want to use your own localmodconfig via:

https://wiki.archlinux.org/title/Modprobed-db


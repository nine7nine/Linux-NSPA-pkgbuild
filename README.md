# Linux-NSPA:

![My Image](/images/linux-nspa-banner.png)

### Linux-NSPA Archlinux Packages

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google, Kernel Toast, upstream and various other sources.

### Features/Patchwork:

* PREEMPT_RT_FULL : Realtime Linux Patchset
* Fair/RT Scheduler optimizations, modifications + backports
* Multi-Gnerational LRU (https://lwn.net/Articles/856931/)
* Tunable WorkingSet Protection Mechanism 
* Winesync driver (Although currently Fsync/Futex_waitv is better)
* Subset of Intel Clear Linux Kernel patches
* Various Performance / interactivity related changes
* Wine-related performance patchwork
* Power management improvements
* Numerous subsystem backports from 5.19+
* Faster bootup
* Misc fixes (nvme, xhci, mm, pm, locking, etc)
* ioprio patchset
* rtw88 related patchwork

NOTE: currently sticking with 5.18+ kernel, until linux-6.1 is available for rebase (Maple tree + MLGru, etc)

SPECIAL NOTE: the included kernel config is specifically for my laptop. If
anyone is using these packages, you will need to have a look at the 
'config_generic_nspa' config file included. -- you can use it directly, use it as a 
reference OR use it in combination with modprobed-db + make localmodconfig.

see commit: https://github.com/nine7nine/Linux-NSPA-pkgbuild/commit/10b12669a7086c3ed9634569171e9b4fa448000b

Linux-NSPA kernel sources can be found here: https://github.com/nine7nine/Linux-NSPA

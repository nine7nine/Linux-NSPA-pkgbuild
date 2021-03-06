# Linux-NSPA:

![My Image](/images/linux-nspa-banner.png)

### Linux-NSPA Archlinux Packages

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google annd other sources.

### Features/Patchwork:

* PREEMPT_RT_FULL : Realtime Linux Patchset
* Multi-Gnerational LRU (https://lwn.net/Articles/856931/)
* Tunable WorkingSet Protection Mechanism 
* Winesync driver (Although currently Fsync/Futex_waitv is better)
* Subset of Intel Clear Linux Kernel patches
* Various Performance / interactivity related changes
* Wine-related patchwork
* Power management improvements
* Faster bootup
* Misc fixes

SPECIAL NOTE: the included kernel config is specifically for my laptop. If
anyone is using these packages, you will need to have a look at the 
'config_generic_nspa' config file included. -- you can use it directly, use it as a 
reference OR use it in combination with modprobed-db + make localmodconfig.

see commit: https://github.com/nine7nine/Linux-NSPA-pkgbuild/commit/10b12669a7086c3ed9634569171e9b4fa448000b

Linux-NSPA kernel sources can be found here: https://github.com/nine7nine/Linux-NSPA

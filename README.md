# LINUX-NSPA

![My Image](/images/linux-nspa-banner.png)

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google annd other sources.

## My patch list;

* 0001-arch.patch
* 0002-anbox.patch
* 0003-bbr2.patch
* 0004-cachy.patch
* 0005-migrate.patch
* 0006-clearlinux.patch
* 0007-cpu.patch
* 0008-fixes-miscellaneous.patch
* 0009-fs-patches.patch
* 0010-hwmon.patch
* 0015-ck-hrtimer.patch
* 0016-mm-Support-soft-dirty-flag-reset-for-VA-range.patch
* 0017-mm-Support-soft-dirty-flag-read-with-reset.patch
* 0018-sched-fair-Compile-out-NUMA-code-entirely-when-NUMA-.patch
* 0019-x86-Enable-fast-strings-on-Intel-if-BIOS-hasn-t-alre.patch
* 0020-amd_pinctrl-IRQF_NO_THREAD.patch
* 0021-designware-i2c_IRQF_NO_THREAD.patch
* 0022-background_reclaim_of_hugepages.patch
* 0023-patch-5.17.1-rt17.patch
* 0024-Reduce-SCHED_RR-timeslice-100-ms-10-jiffy.patch
* 0025-v5.17-winesync.patch
* 0026-mm.patch
* 0027-mm-MG-Lru-5.17.y-patchset.patch
* 0028-mm-vmscan-add-sysctl-knobs-for-protecting-the-workin.patch

NOTE: the included kernel config is specifically for my laptop. If
anyone is using these packages, you will have to generate your own config.

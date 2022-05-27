# Linux-NSPA:

![My Image](/images/linux-nspa-banner.png)

This repo contains customized PREEMPT_RT kernel packages that have additional
patchwork and out-of-tree features added. Patchwork taken from CachyOS, Intel,
Google annd other sources.

## My patch list;

* 000001-arch.patch
* 000002-acpi_cppc-amd-pstate.patch
* 000003-bbr2.patch
* 000004-cachy.patch
* 000005-peterz-sched-migrate.patch
* 000006-clearlinux-all.patch
* 000007-more-uarches-for-kernel-5.17+.patch
* 000008-fixes-miscellaneous.patch
* 000009-fs-patches.patch
* 000010-hwmon.patch
* 000015-ck-hrtimer.patch
* 000016-mm-Support-soft-dirty-flag-reset-for-VA-range.patch
* 000017-mm-Support-soft-dirty-flag-read-with-reset.patch
* 000018-sched-fair-Compile-out-NUMA-code-entirely-when-NUMA-.patch
* 000019-x86-Enable-fast-strings-on-Intel-if-BIOS-hasn-t-alre.patch
* 000020-amd_pinctrl-IRQF_NO_THREAD.patch
* 000021-designware-i2c_IRQF_NO_THREAD.patch
* 000022-background_reclaim_of_hugepages.patch
* 000023-patch-5.17.1-rt17.patch
* 000024-Reduce-SCHED_RR-timeslice-100-ms-10-jiffy.patch
* 000025-v5.17-winesync.patch
* 000026-mm-ncrease_max_map_count.patch
* 000027-mm-MG-Lru-5.17.y-patchset.patch
* 000028-mm-vmscan-add-sysctl-knobs-for-protecting-the-workin.patch

NOTE: the included kernel config is specifically for my laptop. If
anyone is using these packages, you will have to generate your own config.

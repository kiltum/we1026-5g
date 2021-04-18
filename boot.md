# here is boot log of openwrt
```
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.000000] Linux version 4.14.206 (buildbot@d6b0edf6d597) (gcc version 7.3.0 (OpenWrt GCC 7.3.0 r8077-7cbbab7246)) #0 Wed Nov 11 20:09:58 2020
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Board has DDR2
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Analog PMU set to hw control
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Digital PMU set to hw control
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] SoC Type: MediaTek MT7620A ver:2 eco:6
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] bootconsole [early0] enabled
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] CPU0 revision is: 00019650 (MIPS 24KEc)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] MIPS: machine is ZBT WE1026-5G (16M)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Determined physical RAM map:
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000]  memory: 08000000 @ 00000000 (usable)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Initrd not found or empty - disabling initrd
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    0.000000] Primary instruction cache 64kB, VIPT, 4-way, linesize 32 bytes.
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    0.000000] Primary data cache 32kB, 4-way, PIPT, no aliases, linesize 32 bytes
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Zone ranges:
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000]   Normal   [mem 0x0000000000000000-0x0000000007ffffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Movable zone start for each node
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Early memory node ranges
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000]   node   0: [mem 0x0000000000000000-0x0000000007ffffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Initmem setup node 0 [mem 0x0000000000000000-0x0000000007ffffff]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000] On node 0 totalpages: 32768
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000] free_area_init_node: node 0, pgdat 80427620, node_mem_map 81000040
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000]   Normal zone: 256 pages used for memmap
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000]   Normal zone: 0 pages reserved
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000]   Normal zone: 32768 pages, LIFO batch:7
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.000000] random: get_random_bytes called from 0x8042a730 with crng_init=0
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000] pcpu-alloc: s0 r0 d32768 u32768 alloc=1*32768
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.000000] pcpu-alloc: [0] 0
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Built 1 zonelists, mobility grouping on.  Total pages: 32512
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.000000] Kernel command line: console=ttyS0,115200 rootfstype=squashfs,jffs2
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] PID hash table entries: 512 (order: -1, 2048 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Dentry cache hash table entries: 16384 (order: 4, 65536 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Inode-cache hash table entries: 8192 (order: 3, 32768 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Writing ErrCtl register=0007215c
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Readback ErrCtl register=0007215c
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] Memory: 125128K/131072K available (3609K kernel code, 182K rwdata, 464K rodata, 216K init, 215K bss, 5944K reserved, 0K cma-reserved)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] SLUB: HWalign=32, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] NR_IRQS: 256
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] CPU Clock: 580MHz
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] clocksource: systick: mask: 0xffff max_cycles: 0xffff, max_idle_ns: 583261500 ns
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] systick: enable autosleep mode
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] systick: running - mult: 214748, shift: 32
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000000] clocksource: MIPS: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 6590553264 ns
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.000011] sched_clock: 32 bits at 290MHz, resolution 3ns, wraps every 7405115902ns
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.007608] Calibrating delay loop... 385.84 BogoMIPS (lpj=1929216)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.073547] pid_max: default: 32768 minimum: 301
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.078279] Mount-cache hash table entries: 1024 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.084659] Mountpoint-cache hash table entries: 1024 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.097515] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 19112604462750000 ns
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.107057] futex hash table entries: 256 (order: -1, 3072 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.113048] pinctrl core: initialized pinctrl subsystem
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.119412] NET: Registered protocol family 16
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.604264] PCI host bridge /pcie@10140000 ranges:
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.608881]  MEM 0x0000000020000000..0x000000002fffffff
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.613931]   IO 0x0000000010160000..0x000000001016ffff
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.636619] rt2880_gpio 10000600.gpio: registering 24 gpios
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.642075] rt2880_gpio 10000600.gpio: registering 24 irq handlers
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.648401] rt2880_gpio 10000660.gpio: registering 32 gpios
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.653824] rt2880_gpio 10000660.gpio: registering 32 irq handlers
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.660118] rt2880_gpio 10000688.gpio: registering 1 gpios
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.665457] rt2880_gpio 10000688.gpio: registering 1 irq handlers
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.672204] PCI host bridge to bus 0000:00
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.676181] pci_bus 0000:00: root bus resource [mem 0x20000000-0x2fffffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.682797] pci_bus 0000:00: root bus resource [io  0xffffffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.688557] pci_bus 0000:00: root bus resource [??? 0x00000000 flags 0x0]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.695141] pci_bus 0000:00: No busn resource found for root bus, will use [bus 00-ff]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.702887] pci 0000:00:00.0: [1814:0801] type 01 class 0x060400
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.702933] pci 0000:00:00.0: reg 0x10: [mem 0x00000000-0x7fffffff]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.702949] pci 0000:00:00.0: reg 0x14: [mem 0x00000000-0x0000ffff]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.703034] pci 0000:00:00.0: supports D1
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.703046] pci 0000:00:00.0: PME# supported from D0 D1 D3hot
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.703326] pci 0000:00:00.0: bridge configuration invalid ([bus 00-00]), reconfiguring
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711237] pci 0000:01:00.0: [14c3:7662] type 00 class 0x028000
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711302] pci 0000:01:00.0: reg 0x10: [mem 0x00000000-0x000fffff 64bit]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711357] pci 0000:01:00.0: reg 0x30: [mem 0x00000000-0x0000ffff pref]
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711468] pci 0000:01:00.0: PME# supported from D0 D3hot D3cold
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711699] pci_bus 0000:01: busn_res: [bus 01-ff] end is updated to 01
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.711721] pci_bus 0000:00: busn_res: [bus 00-ff] end is updated to 01
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.711774] pci 0000:00:00.0: BAR 0: no space for [mem size 0x80000000]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.718191] pci 0000:00:00.0: BAR 0: failed to assign [mem size 0x80000000]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.724904] pci 0000:00:00.0: BAR 8: assigned [mem 0x20000000-0x200fffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.731509] pci 0000:00:00.0: BAR 9: assigned [mem 0x20100000-0x201fffff pref]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.738511] pci 0000:00:00.0: BAR 1: assigned [mem 0x20200000-0x2020ffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.745125] pci 0000:01:00.0: BAR 0: assigned [mem 0x20000000-0x200fffff 64bit]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.752217] pci 0000:01:00.0: BAR 6: assigned [mem 0x20100000-0x2010ffff pref]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.759229] pci 0000:00:00.0: PCI bridge to [bus 01]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.764038] pci 0000:00:00.0:   bridge window [mem 0x20000000-0x200fffff]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.770641] pci 0000:00:00.0:   bridge window [mem 0x20100000-0x201fffff pref]
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.782532] clocksource: Switched to clocksource systick
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.788842] NET: Registered protocol family 2
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.794102] TCP established hash table entries: 1024 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.800829] TCP bind hash table entries: 1024 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.807050] TCP: Hash tables configured (established 1024 bind 1024)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.813321] UDP hash table entries: 256 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.818949] UDP-Lite hash table entries: 256 (order: 0, 4096 bytes)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.825331] NET: Registered protocol family 1
Wed Nov 11 20:10:03 2020 kern.debug kernel: [    0.829564] PCI: CLS 0 bytes, default 32
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.832261] rt-timer 10000100.timer: maximum frequency is 1220Hz
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    0.838992] Crashlog allocated RAM at address 0x3f00000
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.845790] workingset: timestamp_bits=30 max_order=15 bucket_order=0
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.858092] squashfs: version 4.0 (2009/01/31) Phillip Lougher
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.863740] jffs2: version 2.2 (NAND) (SUMMARY) (LZMA) (RTIME) (CMODE_PRIORITY) (c) 2001-2006 Red Hat, Inc.
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.883599] io scheduler noop registered
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.887347] io scheduler deadline registered (default)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.893376] Serial: 8250/16550 driver, 16 ports, IRQ sharing enabled
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.902497] console [ttyS0] disabled
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.906015] 10000c00.uartlite: ttyS0 at MMIO 0x10000c00 (irq = 20, base_baud = 2500000) is a Palmchip BK-3103
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.915646] console [ttyS0] enabled
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.922696] bootconsole [early0] disabled
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    0.938901] spi spi0.0: force spi mode3
Wed Nov 11 20:10:03 2020 kern.info kernel: [    0.952609] m25p80 spi0.0: w25q128 (16384 Kbytes)
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.957465] 4 fixed-partitions partitions found on MTD device spi0.0
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.963963] Creating 4 MTD partitions on "spi0.0":
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.968860] 0x000000000000-0x000000030000 : "u-boot"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.974885] 0x000000030000-0x000000040000 : "u-boot-env"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.981158] 0x000000040000-0x000000050000 : "factory"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    0.987260] 0x000000050000-0x000001000000 : "firmware"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.722514] random: fast init done
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.869097] 2 uimage-fw partitions found on MTD device firmware
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.875172] 0x000000050000-0x0000001b0bc4 : "kernel"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.881126] 0x0000001b0bc4-0x000001000000 : "rootfs"
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.887075] mtd: device 5 (rootfs) set to be root filesystem
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.894447] 1 squashfs-split partitions found on MTD device rootfs
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    2.900780] 0x000000419000-0x000001000000 : "rootfs_data"
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.907998] libphy: Fixed MDIO Bus: probed
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.917004] gsw: setting port4 to ephy mode
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.921541] mtk_soc_eth 10100000.ethernet: loaded mt7620 driver
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.928340] mtk_soc_eth 10100000.ethernet eth0: mediatek frame engine at 0xb0100000, irq 5
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.937345] rt2880_wdt 10000120.watchdog: Initialized
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.943953] NET: Registered protocol family 10
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.952602] Segment Routing with IPv6
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.956475] NET: Registered protocol family 17
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.961069] bridge: filtering via arp/ip/ip6tables is no longer available by default. Update your scripts to load br_netfilter if you need this.
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.974324] 8021q: 802.1Q VLAN Support v1.8
Wed Nov 11 20:10:03 2020 kern.info kernel: [    2.994679] VFS: Mounted root (squashfs filesystem) readonly on device 31:5.
Wed Nov 11 20:10:03 2020 kern.info kernel: [    3.003117] Freeing unused kernel memory: 216K
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    3.007654] This architecture does not have kernel memory protection.
Wed Nov 11 20:10:03 2020 user.info kernel: [    4.464228] init: Console is alive
Wed Nov 11 20:10:03 2020 user.info kernel: [    4.467944] init: - watchdog -
Wed Nov 11 20:10:03 2020 user.info kernel: [    6.648327] kmodloader: loading kernel modules from /etc/modules-boot.d/*
Wed Nov 11 20:10:03 2020 kern.info kernel: [    6.967139] usbcore: registered new interface driver usbfs
Wed Nov 11 20:10:03 2020 kern.info kernel: [    6.972924] usbcore: registered new interface driver hub
Wed Nov 11 20:10:03 2020 kern.info kernel: [    6.978453] usbcore: registered new device driver usb
Wed Nov 11 20:10:03 2020 kern.info kernel: [    6.989484] ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
Wed Nov 11 20:10:03 2020 kern.info kernel: [    6.997900] ehci-platform: EHCI generic platform driver
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.013667] phy phy-usbphy.0: remote usb device wakeup disabled
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.019715] phy phy-usbphy.0: UTMI 16bit 30MHz
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.024279] ehci-platform 101c0000.ehci: EHCI Host Controller
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.030191] ehci-platform 101c0000.ehci: new USB bus registered, assigned bus number 1
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.038405] ehci-platform 101c0000.ehci: irq 26, io mem 0x101c0000
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.054346] ehci-platform 101c0000.ehci: USB 2.0 started, EHCI 1.00
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.061778] hub 1-0:1.0: USB hub found
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.066078] hub 1-0:1.0: 1 port detected
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.073367] ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.081301] ohci-platform: OHCI generic platform driver
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.087014] ohci-platform 101c1000.ohci: Generic Platform OHCI controller
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.093973] ohci-platform 101c1000.ohci: new USB bus registered, assigned bus number 2
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.102202] ohci-platform 101c1000.ohci: irq 26, io mem 0x101c1000
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.135981] hub 2-0:1.0: USB hub found
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.140265] hub 2-0:1.0: 1 port detected
Wed Nov 11 20:10:03 2020 kern.warn kernel: [    7.156907] MTK MSDC device init.
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.178211] mtk-sd: MediaTek MT6575 MSDC Driver
Wed Nov 11 20:10:03 2020 user.info kernel: [    7.187272] kmodloader: done loading kernel modules from /etc/modules-boot.d/*
Wed Nov 11 20:10:03 2020 user.info kernel: [    7.198979] init: - preinit -
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.352045] usb 1-1: new high-speed USB device number 2 using ehci-platform
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.569721] hub 1-1:1.0: USB hub found
Wed Nov 11 20:10:03 2020 kern.info kernel: [    7.575156] hub 1-1:1.0: 4 ports detected
Wed Nov 11 20:10:03 2020 kern.notice kernel: [    8.144038] random: procd: uninitialized urandom read (4 bytes read)
Wed Nov 11 20:10:03 2020 kern.info kernel: [    8.465848] usb 1-1.2: new high-speed USB device number 3 using ehci-platform
Wed Nov 11 20:10:03 2020 kern.info kernel: [    9.181593] 8021q: adding VLAN 0 to HW filter on device eth0
Wed Nov 11 20:10:03 2020 user.notice kernel: [   10.493603] mount_root: jffs2 not ready yet, using temporary tmpfs overlay
Wed Nov 11 20:10:03 2020 user.warn kernel: [   10.533649] urandom-seed: Seed file not found (/etc/urandom.seed)
Wed Nov 11 20:10:03 2020 user.info kernel: [   10.652377] procd: - early -
Wed Nov 11 20:10:03 2020 user.info kernel: [   10.655441] procd: - watchdog -
Wed Nov 11 20:10:03 2020 user.info kernel: [   11.115881] procd: - watchdog -
Wed Nov 11 20:10:03 2020 user.info kernel: [   11.119422] procd: - ubus -
Wed Nov 11 20:10:03 2020 kern.notice kernel: [   11.342188] random: ubusd: uninitialized urandom read (4 bytes read)
Wed Nov 11 20:10:03 2020 kern.notice kernel: [   11.521802] random: ubusd: uninitialized urandom read (4 bytes read)
Wed Nov 11 20:10:03 2020 kern.notice kernel: [   11.528897] random: ubusd: uninitialized urandom read (4 bytes read)
Wed Nov 11 20:10:03 2020 user.info kernel: [   11.536493] procd: - init -
Wed Nov 11 20:10:03 2020 user.info kernel: [   11.914530] kmodloader: loading kernel modules from /etc/modules.d/*
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.021920] ip6_tables: (C) 2000-2006 Netfilter Core Team
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.040195] Loading modules backported from Linux version wt-2017-11-01-0-gfe248fc2c180
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.048461] Backport generated by backports.git v4.14-rc2-1-31-g86cf0e5d
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.059690] ip_tables: (C) 2000-2006 Netfilter Core Team
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.074798] nf_conntrack version 0.5.0 (2048 buckets, 8192 max)
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.150251] xt_time: kernel timezone is -0000
Wed Nov 11 20:10:03 2020 kern.err kernel: [   12.225491] mt76x2e 0000:01:00.0: card - bus=0x1, slot = 0x0 irq=4
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.232086] mt76x2e 0000:01:00.0: ASIC revision: 76120044
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.458749] mt76x2e 0000:01:00.0: ROM patch build: 20141115060606a
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.470942] mt76x2e 0000:01:00.0: Firmware Version: 0.0.00
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.476608] mt76x2e 0000:01:00.0: Build: 1
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.480790] mt76x2e 0000:01:00.0: Build Time: 201507311614____
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.495577] mt76x2e 0000:01:00.0: Firmware running!
Wed Nov 11 20:10:03 2020 kern.debug kernel: [   12.501620] ieee80211 phy0: Selected rate control algorithm 'minstrel_ht'
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.528556] PPP generic driver version 2.4.2
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.539231] NET: Registered protocol family 24
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.657144] rt2800_wmac 10180000.wmac: loaded eeprom from mtd device "factory"
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.664539] ieee80211 phy1: rt2x00_set_rt: Info - RT chipset 6352, rev 0500 detected
Wed Nov 11 20:10:03 2020 kern.info kernel: [   12.672522] ieee80211 phy1: rt2x00_set_rf: Info - RF chipset 7620 detected
Wed Nov 11 20:10:03 2020 kern.debug kernel: [   12.680247] ieee80211 phy1: Selected rate control algorithm 'minstrel_ht'
Wed Nov 11 20:10:03 2020 user.info kernel: [   12.686306] kmodloader: done loading kernel modules from /etc/modules.d/*
Wed Nov 11 20:10:03 2020 kern.warn kernel: [   14.154999] urandom_read: 5 callbacks suppressed
Wed Nov 11 20:10:03 2020 kern.notice kernel: [   14.155010] random: jshn: uninitialized urandom read (4 bytes read)
Wed Nov 11 20:10:04 2020 user.notice dnsmasq: DNS rebinding protection is active, will discard upstream RFC1918 responses!
Wed Nov 11 20:10:04 2020 user.notice dnsmasq: Allowing 127.0.0.0/8 responses
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: started, version 2.80 cachesize 150
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: DNS service limited to local subnets
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: compile time options: IPv6 GNU-getopt no-DBus no-i18n no-IDN DHCP no-DHCPv6 no-Lua TFTP no-conntrack no-ipset no-auth no-DNSSEC no-ID loop-detect inotify dumpfile
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain test
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain onion
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain localhost
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain local
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain invalid
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain bind
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: using local addresses only for domain lan
Wed Nov 11 20:10:05 2020 daemon.warn dnsmasq[943]: no servers found in /tmp/resolv.conf.auto, will retry
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: read /etc/hosts - 4 addresses
Wed Nov 11 20:10:05 2020 daemon.info dnsmasq[943]: read /tmp/hosts/dhcp.cfg01411c - 0 addresses
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: tunnel
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: Network device
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: bridge
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: veth
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: macvlan
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: 8021ad
Wed Nov 11 20:10:08 2020 user.notice : Added device handler type: 8021q
Wed Nov 11 20:10:08 2020 daemon.notice procd: /etc/init.d/network: 'radio0' is disabled
Wed Nov 11 20:10:08 2020 daemon.notice procd: /etc/init.d/network: 'radio1' is disabled
Wed Nov 11 20:10:08 2020 daemon.notice procd: /etc/init.d/network: 'radio0' is disabled
Wed Nov 11 20:10:08 2020 daemon.notice procd: /etc/init.d/network: 'radio1' is disabled
Wed Nov 11 20:10:11 2020 user.notice ucitrack: Setting up /etc/config/network reload dependency on /etc/config/dhcp
Wed Nov 11 20:10:11 2020 user.notice ucitrack: Setting up /etc/config/network reload dependency on /etc/config/radvd
Wed Nov 11 20:10:11 2020 user.notice ucitrack: Setting up /etc/config/wireless reload dependency on /etc/config/network
Wed Nov 11 20:10:12 2020 user.notice ucitrack: Setting up /etc/config/firewall reload dependency on /etc/config/luci-splash
Wed Nov 11 20:10:12 2020 user.notice ucitrack: Setting up /etc/config/firewall reload dependency on /etc/config/qos
Wed Nov 11 20:10:12 2020 user.notice ucitrack: Setting up /etc/config/firewall reload dependency on /etc/config/miniupnpd
Wed Nov 11 20:10:12 2020 user.notice ucitrack: Setting up /etc/config/dhcp reload dependency on /etc/config/odhcpd
Wed Nov 11 20:10:13 2020 user.notice ucitrack: Setting up non-init /etc/config/fstab reload handler: /sbin/block mount
Wed Nov 11 20:10:13 2020 user.notice ucitrack: Setting up /etc/config/system reload trigger for non-procd /etc/init.d/led
Wed Nov 11 20:10:13 2020 user.notice ucitrack: Setting up /etc/config/system reload dependency on /etc/config/luci_statistics
Wed Nov 11 20:10:13 2020 user.notice ucitrack: Setting up /etc/config/system reload dependency on /etc/config/dhcp
Wed Nov 11 20:10:15 2020 kern.warn kernel: [   28.390611] jffs2_scan_eraseblock(): End of filesystem marker found at 0x0
Wed Nov 11 20:10:15 2020 kern.warn kernel: [   28.416657] jffs2_build_filesystem(): unlocking the mtd device...
Wed Nov 11 20:10:15 2020 kern.warn kernel: [   28.416734] done.
Wed Nov 11 20:10:15 2020 kern.warn kernel: [   28.425008] jffs2_build_filesystem(): erasing all blocks after the end marker...
Wed Nov 11 20:10:15 2020 kern.info kernel: [   28.885945] 8021q: adding VLAN 0 to HW filter on device eth0
Wed Nov 11 20:10:15 2020 kern.info kernel: [   28.951637] br-lan: port 1(eth0.1) entered blocking state
Wed Nov 11 20:10:15 2020 kern.info kernel: [   28.957403] br-lan: port 1(eth0.1) entered disabled state
Wed Nov 11 20:10:15 2020 kern.info kernel: [   28.963274] device eth0.1 entered promiscuous mode
Wed Nov 11 20:10:15 2020 kern.info kernel: [   28.968224] device eth0 entered promiscuous mode
Wed Nov 11 20:10:15 2020 kern.info kernel: [   29.069808] br-lan: port 1(eth0.1) entered blocking state
Wed Nov 11 20:10:15 2020 kern.info kernel: [   29.075336] br-lan: port 1(eth0.1) entered forwarding state
Wed Nov 11 20:10:15 2020 kern.info kernel: [   29.081313] IPv6: ADDRCONF(NETDEV_UP): br-lan: link is not ready
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'lan' is enabled
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'lan' is setting up now
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'lan' is now up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'loopback' is enabled
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'loopback' is setting up now
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'loopback' is now up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: bridge 'br-lan' link is up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'lan' has link connectivity
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Network device 'eth0' link is up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: VLAN 'eth0.1' link is up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Network device 'lo' link is up
Wed Nov 11 20:10:15 2020 daemon.notice netifd: Interface 'loopback' has link connectivity
Wed Nov 11 20:10:16 2020 user.notice firewall: Reloading firewall due to ifup of lan (br-lan)
Wed Nov 11 20:10:16 2020 kern.info kernel: [   29.945779] IPv6: ADDRCONF(NETDEV_CHANGE): br-lan: link becomes ready
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[943]: exiting on receipt of SIGTERM
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: started, version 2.80 cachesize 150
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: DNS service limited to local subnets
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: compile time options: IPv6 GNU-getopt no-DBus no-i18n no-IDN DHCP no-DHCPv6 no-Lua TFTP no-conntrack no-ipset no-auth no-DNSSEC no-ID loop-detect inotify dumpfile
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq-dhcp[1358]: DHCP, IP range 192.168.1.100 -- 192.168.1.249, lease time 12h
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain test
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain onion
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain localhost
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain local
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain invalid
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain bind
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: using local addresses only for domain lan
Wed Nov 11 20:10:22 2020 daemon.warn dnsmasq[1358]: no servers found in /tmp/resolv.conf.auto, will retry
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: read /etc/hosts - 4 addresses
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq[1358]: read /tmp/hosts/dhcp.cfg01411c - 2 addresses
Wed Nov 11 20:10:22 2020 daemon.info dnsmasq-dhcp[1358]: read /etc/ethers - 0 addresses
Wed Nov 11 20:10:23 2020 daemon.info dnsmasq[1358]: read /etc/hosts - 4 addresses
Wed Nov 11 20:10:23 2020 daemon.info dnsmasq[1358]: read /tmp/hosts/dhcp.cfg01411c - 2 addresses
Wed Nov 11 20:10:23 2020 daemon.info dnsmasq-dhcp[1358]: read /etc/ethers - 0 addresses
Wed Nov 11 20:10:57 2020 authpriv.info dropbear[1406]: Not backgrounding
Wed Nov 11 20:11:03 2020 kern.notice kernel: [   76.662366] random: crng init done
```

Waits some

```
Wed Nov 11 20:13:01 2020 kern.warn kernel: [  194.830260] done.
Wed Nov 11 20:13:01 2020 kern.notice kernel: [  194.832279] jffs2: notice: (1210) jffs2_build_xattr_subsystem: complete building xattr subsystem, 0 of xdatum (0 unchecked, 0 orphan) and 0 of xref (0 dead, 0 orphan) found.
Wed Nov 11 20:13:01 2020 daemon.info mount_root: performing overlay whiteout
Wed Nov 11 20:13:01 2020 daemon.info mount_root: syncronizing overlay
Wed Nov 11 20:13:01 2020 kern.warn kernel: [  195.092756] overlayfs: upper fs does not support tmpfile.
Wed Nov 11 20:13:01 2020 daemon.err mount_root: failed to sync jffs2 overlay
Wed Nov 11 20:13:02 2020 daemon.notice procd: /etc/rc.d/S96led: setting up led LAN
Wed Nov 11 20:13:02 2020 daemon.notice procd: /etc/rc.d/S96led: setting up led wifi
Wed Nov 11 20:13:02 2020 daemon.notice procd: /etc/rc.d/S96led: setting up led USB
Wed Nov 11 20:13:02 2020 daemon.notice procd: /etc/rc.d/S96led: Skipping trigger 'usbport' for led 'USB' due to missing kernel module
Wed Nov 11 20:13:02 2020 daemon.info procd: - init complete -
Wed Nov 11 20:13:03 2020 daemon.info urandom_seed[1496]: Seed saved (/etc/urandom.seed)
```

and right after this reboots


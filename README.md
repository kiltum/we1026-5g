# WE1026-5G

Potentially good router, but does not work at all. Many mistakes in config scripts.

SSH available on 2222 port, but no credentials yet

## Get firmware for restoration

1. Telnet to 192.168.1.1 with admin/admin and get castrated console, where you can do nothing
2. But you can call ps, look at something like this
```
wget -T 15 -t 1 --no-check-certificate https://ac-link.com/upgrade/WE1026-5G/latest.txt.en?sn=f8:5e:3c:1e:xx:xx -O /tmp/latest.txt -o /tmp/wget.log
```
3. Download it and open
```
$ cat latest.txt.en\?sn\=f8\:5e\:3c\:1e\:xx\:xx 
latest=19.1101
release_time=2019-11-01 23:34:35
url=https://ac-link.com/upgrade/WE1026-5G/mt7620-WE1026-5G-20191101_233435.bin
changelog=19.11.01\nUpdate logs\n1. Fix the possible dial failure bug caused by simcom module configuring APN\n2. Fix the bug that APN cannot be cleared in the 
....
Many strings ommitted
```
4. Now download firmware
```
wget https://ac-link.com/upgrade/WE1026-5G/mt7620-WE1026-5G-20191101_233435.bin
```

## How to restore from brick

1. Download firmware as described above
2. Connect Ethernet cable to brick, set own ip to some in 192.168.1.0/24 network. 
3. Start ping 192.168.1.1
4. Power on router with pressed reset button
5. wait 3-4 sec, unpress reset
6. point browser to 192.168.1.1 and upload bin file. 
OR
6. ask curl to do this. REPLACE 2.bin to your file name (NOTE: No pings during upload) 
```
curl -i -X POST -H "Content-Type: multipart/form-data" -F "firmware=@2.bin" http://192.168.1.1/
``` 

7. Wait for some time, router will reboot automatically

PS: Log of process also shows thru serial

## How to get selial console

1. Unscrew router from antenna side
2. Pull out mother board
3. Connect serial terminal to RX/TX/GND pins
4. Open terminal at port with 115200/8/1
5. Press Enter

## Boot log after flashing

```
U-Boot 1.1.3 (Jan 23 2015 - 17:03:11)

SoC:MediaTek MT7620
DRAM:  Memory Testing..131072K OK. is 128 MB
relocate_code Pointer at: 87fb0000
enable ephy clock...done. rf reg 29 = 5
SSC disabled.
spi_wait_nsec: 29
spi device id: ef 40 18 0 0 (40180000)
Flash: W25Q128BV
*** Warning - bad CRC, using default environment

 _______________________________________________________________
|    ____                 _                 ____               |
|   |  _ \ __ _ _ __   __| | ___  _ __ __ _| __ )  _____  __   |
|   | |_) / _` | '_ \ / _` |/ _ \| '__/ _` |  _ \ / _ \ \/ /   |
|   |  __/ (_| | | | | (_| | (_) | | | (_| | |_) | (_) >  <    |
|   |_|   \__,_|_| |_|\__,_|\___/|_|  \__,_|____/ \___/_/\_\   |
|                                                              |
|                  Ralink/MTK SDK Plantform                    |
|                    Copyright 2005-2013                       |
|                    Board:MTK MT7620A EVB                     |
===============System Info==================
ASIC 7620_MP (Port5<->None)
DRAM component: 1024 Mbits DDR, width 16
DRAM bus: 16 bit
Flash component: SPI Flash
CPU Speed: 580 MHZ
RAM Size:128 Mbytes

Build Date:Jan 23 2015  Time:17:03:11
============================================

GSW VLAN:LLLW

GPIO Init:
        UARTF_SHARE_MODE:GPIO
        I2C_GPIO_MODE:GPIO
init gpio20!
----------------------------------------

 64M-ROM------------------------
Uboot version 1.3 ---zbt826-64M flash

---------------------------------------
GPIO_MODE_REG:0x1a311d
ReadyLED Bit:0x200

Please choose the operation:
   1: Load system code to SDRAM via TFTP.
   2: Load system code then write to Flash via TFTP.
   3: Boot system code via Flash (default).
   4: Entr boot command line interface.
   7: Load Boot Loader code then write to Flash via Serial.
   9: Load Boot Loader code then write to Flash via TFTP.                     0

3: System Boot system code via Flash.

Press Reset button enter upgrade mode!

Reset button pressed!


 NetTxPacket = 0x87FE47C0

 KSEG1ADDR(NetTxPacket) = 0xA7FE47C0

 NetLoop,call eth_halt !
Trying Eth0 (10/100-M)

 Waitting for RX_DMA_BUSY status Start... done


 ETH_STATE_ACTIVE!!
uHttpd Server started.
IP:192.168.1.1
Netmask:255.255.255.0
Default Router:0.0.0.0
expecting 9437389 bytes

=================================================

Check image:
Image type              --> Firmware
Image Header Checksum   --> OK
Image Data Checksum     --> OK

=================================================
Bytes transferred = 9437188 (900004 hex)
Upgrade linux kernel block !!
................................................................................................................................................
................................................................................................................................................
.
.
Done!
```

## First boot


```
U-Boot 1.1.3 (Jan 23 2015 - 17:03:11)

SoC:MediaTek MT7620
DRAM:  Memory Testing..131072K OK. is 128 MB
relocate_code Pointer at: 87fb0000
enable ephy clock...done. rf reg 29 = 5
SSC disabled.
******************************
Software System Reset Occurred
******************************
spi_wait_nsec: 29
spi device id: ef 40 18 0 0 (40180000)
Flash: W25Q128BV
*** Warning - bad CRC, using default environment

 _______________________________________________________________
|    ____                 _                 ____               |
|   |  _ \ __ _ _ __   __| | ___  _ __ __ _| __ )  _____  __   |
|   | |_) / _` | '_ \ / _` |/ _ \| '__/ _` |  _ \ / _ \ \/ /   |
|   |  __/ (_| | | | | (_| | (_) | | | (_| | |_) | (_) >  <    |
|   |_|   \__,_|_| |_|\__,_|\___/|_|  \__,_|____/ \___/_/\_\   |
|                                                              |
|                  Ralink/MTK SDK Plantform                    |
|                    Copyright 2005-2013                       |
|                    Board:MTK MT7620A EVB                     |
===============System Info==================
ASIC 7620_MP (Port5<->None)
DRAM component: 1024 Mbits DDR, width 16
DRAM bus: 16 bit
Flash component: SPI Flash
CPU Speed: 580 MHZ
RAM Size:128 Mbytes

Build Date:Jan 23 2015  Time:17:03:11
============================================

GSW VLAN:LLLW

GPIO Init:
        UARTF_SHARE_MODE:GPIO
        I2C_GPIO_MODE:GPIO
init gpio20!
----------------------------------------

 64M-ROM------------------------
Uboot version 1.3 ---zbt826-64M flash

---------------------------------------
GPIO_MODE_REG:0x1a311d
ReadyLED Bit:0x200

Please choose the operation:
   1: Load system code to SDRAM via TFTP.
   2: Load system code then write to Flash via TFTP.
   3: Boot system code via Flash (default).
   4: Entr boot command line interface.
   7: Load Boot Loader code then write to Flash via Serial.
   9: Load Boot Loader code then write to Flash via TFTP.                     0

3: System Boot system code via Flash.

Press Reset button enter upgrade mode!
## Booting image at bc050000 ...
   Image Name:   MQWRT:MTK:WE1026-5G:0
   Image Type:   MIPS Linux Kernel Image (lzma compressed)
   Data Size:    1240327 Bytes =  1.2 MB
   Load Address: 80000000
   Entry Point:  80000000
   Verifying Checksum ... OK
   Uncompressing Kernel Image ... OK
No initrd
## Transferring control to Linux (at address 80000000) ...
## Giving linux memsize in MB, 128

Starting kernel ...

怘▒▒▒▒ff▒▒~▒▒~fx▒▒▒怘▒怘▒f▒▒▒▒▒▒▒▒f▒f▒▒▒怘▒f`▒▒▒▒▒▒f▒▒▒▒[    0.000000] Linux version 3.10.14 (mq@ubt1604) (gcc version 4.8.3 (OpenWrt/Linaro GCC 4.8-2014.04 unknown) ) #818 Tue Mar 26 15:35:06 CST 2019
[    0.000000]
[    0.000000]  The CPU feqenuce set to 580 MHz
[    0.000000]
[    0.000000]  MIPS CPU sleep mode enabled.
[    0.000000]  PCIE: bypass PCIe DLL.
[    0.000000]  PCIE: Elastic buffer control: Addr:0x68 -> 0xB4
[    0.000000]  disable all power about PCIe
[    0.000000] CPU0 revision is: 00019650 (MIPS 24KEc)
[    0.000000] Software DMA cache coherency
[    0.000000] Determined physical RAM map:
[    0.000000]  memory: 08000000 @ 00000000 (usable)
[    0.000000] Initrd not found or empty - disabling initrd
[    0.000000] Zone ranges:
[    0.000000]   Normal   [mem 0x00000000-0x07ffffff]
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x00000000-0x07ffffff]
[    0.000000] Primary instruction cache 64kB, 4-way, VIPT, linesize 32 bytes.
[    0.000000] Primary data cache 32kB, 4-way, PIPT, no aliases, linesize 32 bytes
[    0.000000] Built 1 zonelists in Zone order, mobility grouping on.  Total pages: 32512
[    0.000000] Kernel command line: console=ttyS1,115200n8 root=/dev/mtdblock5 rootfstype=squashfs,jffs2 print-fatal-signals=1
[    0.000000] PID hash table entries: 512 (order: -1, 2048 bytes)
[    0.000000] Dentry cache hash table entries: 16384 (order: 4, 65536 bytes)
[    0.000000] Inode-cache hash table entries: 8192 (order: 3, 32768 bytes)
[    0.000000] Writing ErrCtl register=00072151
[    0.000000] Readback ErrCtl register=00072151
[    0.000000] Memory: 125996k/131072k available (2726k kernel code, 5076k reserved, 692k data, 228k init, 0k highmem)
[    0.000000] NR_IRQS:128
[    0.000000] console [ttyS1] enabled
[    0.096000] Calibrating delay loop... 385.02 BogoMIPS (lpj=770048)
[    0.128000] pid_max: default: 32768 minimum: 301
[    0.132000] Mount-cache hash table entries: 512
[    0.136000] NET: Registered protocol family 16
[    0.140000] RALINK_GPIOMODE = 1a311d
[    0.144000] RALINK_GPIOMODE = 18311d
[    0.144000] PPLL_CFG1=0xe78000
[    0.148000] MT7620 PPLL lock
[    0.148000] PPLL_DRV =0x80080504
[    0.152000] start PCIe register access
[    0.652000] RALINK_RSTCTRL = 2400000
[    0.656000] RALINK_CLKCFG1 = 75afffc0
[    0.656000]
[    0.656000] *************** MT7620 PCIe RC mode *************
[    1.156000] PCIE0 enabled
[    1.160000] Port 0 N_FTS = 1b105000
[    1.160000] init_rt2880pci done
[    1.188000] bio: create slab <bio-0> at 0
[    1.192000] PCI host bridge to bus 0000:00
[    1.196000] pci_bus 0000:00: root bus resource [mem 0x20000000-0x2fffffff]
[    1.200000] pci_bus 0000:00: root bus resource [io  0x10160000-0x1016ffff]
[    1.204000] pci_bus 0000:00: No busn resource found for root bus, will use [bus 00-ff]
[    1.208000] pci 0000:00:00.0: bridge configuration invalid ([bus 00-00]), reconfiguring
[    1.212000] pci 0000:00:00.0: BAR 0: can't assign mem (size 0x80000000)
[    1.216000] pci 0000:00:00.0: BAR 8: assigned [mem 0x20000000-0x200fffff]
[    1.220000] pci 0000:00:00.0: BAR 9: assigned [mem 0x20100000-0x201fffff pref]
[    1.224000] pci 0000:00:00.0: BAR 1: assigned [mem 0x20200000-0x2020ffff]
[    1.228000] pci 0000:01:00.0: BAR 0: assigned [mem 0x20000000-0x200fffff 64bit]
[    1.232000] pci 0000:01:00.0: BAR 6: assigned [mem 0x20100000-0x2010ffff pref]
[    1.236000] pci 0000:00:00.0: PCI bridge to [bus 01]
[    1.240000] pci 0000:00:00.0:   bridge window [mem 0x20000000-0x200fffff]
[    1.244000] pci 0000:00:00.0:   bridge window [mem 0x20100000-0x201fffff pref]
[    1.248000] BAR0 at slot 0 = 0
[    1.248000] bus=0x0, slot = 0x0
[    1.252000] res[0]->start = 0
[    1.252000] res[0]->end = 0
[    1.256000] res[1]->start = 20200000
[    1.256000] res[1]->end = 2020ffff
[    1.260000] res[2]->start = 0
[    1.260000] res[2]->end = 0
[    1.264000] res[3]->start = 0
[    1.264000] res[3]->end = 0
[    1.268000] res[4]->start = 0
[    1.268000] res[4]->end = 0
[    1.272000] res[5]->start = 0
[    1.272000] res[5]->end = 0
[    1.276000] bus=0x1, slot = 0x0
[    1.276000] res[0]->start = 20000000
[    1.280000] res[0]->end = 200fffff
[    1.280000] res[1]->start = 0
[    1.284000] res[1]->end = 0
[    1.284000] res[2]->start = 0
[    1.288000] res[2]->end = 0
[    1.288000] res[3]->start = 0
[    1.292000] res[3]->end = 0
[    1.292000] res[4]->start = 0
[    1.296000] res[4]->end = 0
[    1.296000] res[5]->start = 0
[    1.300000] res[5]->end = 0
[    1.304000] Switching to clocksource Ralink Systick timer
[    1.308000] NET: Registered protocol family 2
[    1.316000] TCP established hash table entries: 1024 (order: 1, 8192 bytes)
[    1.320000] TCP bind hash table entries: 1024 (order: 0, 4096 bytes)
[    1.328000] TCP: Hash tables configured (established 1024 bind 1024)
[    1.336000] TCP: reno registered
[    1.340000] UDP hash table entries: 256 (order: 0, 4096 bytes)
[    1.344000] UDP-Lite hash table entries: 256 (order: 0, 4096 bytes)
[    1.352000] NET: Registered protocol family 1
[    1.356000] MTK/Ralink EHCI/OHCI init.
[    1.364000] squashfs: version 4.0 (2009/01/31) Phillip Lougher
[    1.368000] jffs2: version 2.2. (NAND) (SUMMARY)  (LZMA) (RTIME) (CMODE_PRIORITY) (c) 2001-2006 Red Hat, Inc.
[    1.380000] msgmni has been set to 246
[    1.384000] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 254)
[    1.392000] io scheduler noop registered (default)
[    1.396000] Serial: 8250/16550 driver, 2 ports, IRQ sharing disabled
[    1.404000] serial8250: ttyS0 at MMIO 0x10000500 (irq = 37) is a 16550A
[    1.412000] serial8250: ttyS1 at MMIO 0x10000c00 (irq = 12) is a 16550A
[    1.420000] Ralink gpio driver initialized
[    1.424000] Enable Ralink GDMA Controller Module
[    1.428000] GDMA IP Version=3
[    1.432000] spidrv_major = 217
[    1.444000] brd: module loaded
[    1.452000] deice id : ef 40 18 0 0 (40180000)
[    1.456000] W25Q128BV(ef 40180000) (16384 Kbytes)
[    1.460000] mtd .name = raspi, .size = 0x01000000 (16M) .erasesize = 0x00010000 (64K) .numeraseregions = 0
[    1.472000] Creating 5 MTD partitions on "raspi":
[    1.476000] 0x000000000000-0x000001000000 : "ALL"
[    1.480000] 0x000000000000-0x000000030000 : "Bootloader"
[    1.488000] 0x000000030000-0x000000040000 : "Config"
[    1.496000] 0x000000040000-0x000000050000 : "Factory"
[    1.500000] 0x000000050000-0x000001000000 : "firmware"
[    1.508000] 0x00000017ed47-0x000001000000 : "rootfs"
[    1.512000] mtd: partition "rootfs" must either start or end on erase block boundary or be smaller than an erase block -- forcing read-only
[    1.528000] mtd: partition "rootfs_data" created automatically, ofs=0x940000, len=0x6c0000
[    1.536000] 0x000000940000-0x000001000000 : "rootfs_data"
[    1.544000] tun: Universal TUN/TAP device driver, 1.6
[    1.548000] tun: (C) 1999-2004 Max Krasnyansky <maxk@qualcomm.com>
[    1.556000] rdm_major = 253
[    1.560000] SMACCR1 -- : 0x0000f85e
[    1.564000] SMACCR0 -- : 0x3c1e9166
[    1.568000] Ralink APSoC Ethernet Driver Initilization. v3.1  512 rx/tx descriptors allocated, mtu = 1500!
[    1.576000] SMACCR1 -- : 0x0000f85e
[    1.580000] SMACCR0 -- : 0x3c1e9166
[    1.584000] PROC INIT OK!
[    1.588000] Ralink APSoC Hardware Watchdog Timer
[    1.592000] MTK MSDC device init.
[    1.628000] msdc0 -> set mclk to 0!!! <- msdc_set_mclk() : L<634> PID<kworker/u2:0><0x6>
[    1.636000] mtk-sd: MediaTek MT6575 MSDC Driver
[    1.640000] TCP: cubic registered
[    1.644000] NET: Registered protocol family 10
[    1.648000] NET: Registered protocol family 17
[    1.652000] 8021q: 802.1Q VLAN Support v1.8
[    1.664000] VFS: Mounted root (squashfs filesystem) readonly on device 31:5.
[    1.672000] Freeing unused kernel memory: 228K (80357000 - 80390000)
procd: Console is alive
[    4.700000] usbcore: registered new interface driver usbfs
[    4.704000] usbcore: registered new interface driver hub
[    4.712000] usbcore: registered new device driver usb
[    4.720000] Button Hotplug driver version 0.4.1
[    4.760000] SCSI subsystem initialized
[    4.768000] ehci_hcd: USB 2.0 'Enhanced' Host Controller (EHCI) Driver
[    4.776000] ehci-platform: EHCI generic platform driver
[    4.804000] ehci-platform ehci-platform: EHCI Host Controller
[    4.808000] ehci-platform ehci-platform: new USB bus registered, assigned bus number 1
[    4.816000] ehci-platform ehci-platform: irq 18, io mem 0x101c0000
[    4.836000] ehci-platform ehci-platform: USB 2.0 started, EHCI 1.00
[    4.840000] hub 1-0:1.0: USB hub found
[    4.844000] hub 1-0:1.0: 1 port detected
[    4.852000] ehci-pci: EHCI PCI platform driver
[    4.860000] ohci_hcd: USB 1.1 'Open' Host Controller (OHCI) Driver
[    4.884000] ohci-platform ohci-platform: Generic Platform OHCI Controller
[    4.892000] ohci-platform ohci-platform: new USB bus registered, assigned bus number 2
[    4.900000] ohci-platform ohci-platform: irq 18, io mem 0x101c1000
[    4.968000] hub 2-0:1.0: USB hub found
[    4.972000] hub 2-0:1.0: 1 port detected
[    4.988000] usbcore: registered new interface driver usb-storage
procd: - preinit -
[    5.372000] usb 1-1: new high-speed USB device number 2 using ehci-platform
[    5.892000] hub 1-1:1.0: USB hub found
[    5.896000] hub 1-1:1.0: 4 ports detected
[    6.064000] FFFFFFF8:5E:3C:1E:FFFFFF91:66
[    6.068000] Raeth v3.1 (Tasklet,SkbRecycle)
[    6.072000]
[    6.072000] phy_tx_ring = 0x06d0a000, tx_ring = 0xa6d0a000
[    6.080000]
[    6.080000] phy_rx_ring0 = 0x06d0c000, rx_ring[0] = 0xa6d0c000
[    6.088000]
[    6.088000] phy_rx_ring0 = 0x06d0c000, rx_ring[0] = 0xa6d0c000
[    6.096000] SMACCR1 -- : 0x0000f85e
[    6.100000] SMACCR0 -- : 0x3c1e9166
[    6.104000] ESW: Link Status Changed - Port0 Link UP
[    6.116000] CDMA_CSG_CFG = 81000000
[    6.120000] GDMA1_FWD_CFG = 20710000
[    6.288000] usb 1-1.2: new high-speed USB device number 3 using ehci-platform
mount_root.
emmc_partition_find(0x412008, rootfs_data)
(null) is not created by block2mtd, skip.
[    6.412000] block: attempting to load /etc/config/fstab
[    6.460000] block: extroot: not configured
jffs2 is not ready - marker found
[    6.476000] ra2880stop()...Done
[    6.480000] Free TX/RX Ring Memory!
[    6.496000]
[    6.496000]
[    6.496000] Unsupported Device!
[    6.496000] Vendor=2c7c ProdID=306
[    6.496000] Manufacturer=Quectel Product=EP06-E
[    6.496000]
procd: - early -
procd: - ubus -
procd: - init -
Please press Enter to activate this console.
[    7.524000] l2tp_core: L2TP core driver, V2.0
[    7.528000] l2tp_netlink: L2TP netlink interface
[    7.536000] gre: GRE over IPv4 demultiplexor driver
[    7.544000] ip_gre: GRE over IPv4 tunneling driver
[    7.564000] fuse init (API version 7.22)
[    7.576000] usbcore: registered new interface driver cdc_wdm
[    7.616000] usbcore: registered new interface driver usbserial
[    7.728000] usbcore: registered new interface driver usbserial_generic
[    7.736000] usbserial: USB Serial support registered for generic
[    7.748000] PPP generic driver version 2.4.2
[    7.756000] PPP MPPE Compression module registered
[    7.760000] NET: Registered protocol family 24
[    7.768000] usbcore: registered new interface driver qmi_wwan
[    7.784000] usbcore: registered new interface driver option
[    7.788000] usbserial: USB Serial support registered for GSM modem (1-port)
[    7.796000] option 1-1.2:1.0: GSM modem (1-port) converter detected
[    7.804000] usb 1-1.2: GSM modem (1-port) converter now attached to ttyUSB0
[    7.812000] option 1-1.2:1.1: GSM modem (1-port) converter detected
[    7.820000] usb 1-1.2: GSM modem (1-port) converter now attached to ttyUSB1
[    7.828000] option 1-1.2:1.2: GSM modem (1-port) converter detected
[    7.836000] usb 1-1.2: GSM modem (1-port) converter now attached to ttyUSB2
[    7.844000] option 1-1.2:1.3: GSM modem (1-port) converter detected
[    7.852000] usb 1-1.2: GSM modem (1-port) converter now attached to ttyUSB3
[    9.440000] jffs2_scan_eraseblock(): End of filesystem marker found at 0x0
[    9.448000] jffs2_build_filesystem(): unlocking the mtd device... done.
[    9.456000] jffs2_build_filesystem(): erasing all blocks after the end marker... done.
[   36.616000] jffs2: notice: (590) jffs2_build_xattr_subsystem: complete building xattr subsystem, 0 of xdatum (0 unchecked, 0 orphan) and 0 of xref (0 dead, 0 orphan) found.
procd: - init complete -

```

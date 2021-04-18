# How to flash to openwrt

TL;DR; Status: OpenWRT boots nice , but after about 90 second reboots

## Images

1. https://openwrt.org/toh/hwdata/zbt/zbt_we1026-5g - works, flashed, but reboots



## Image preparing

1. Grab image
2. Open image in hex editor
3. Change name of image to "MQWRT:MTK:WE1026-5G:0" at 0x20
4. Get off image header
```
dd if=image of=header bs=1 count=64
```
5. Claer CRC in image header. Set 4 bytes from 0x4 till 0x8 to 0
6. Calculate CRC
```
crc32 header
```
7. Put those bytes from 0x4 to image


## Console

```
$ ssh root@192.168.1.1
The authenticity of host '192.168.1.1 (192.168.1.1)' can't be established.
RSA key fingerprint is SHA256:K9EQaYpSCIFlExejr9o3lDGyFtgVtaLLxe1JYzWKD00.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '192.168.1.1' (RSA) to the list of known hosts.


BusyBox v1.30.1 () built-in shell (ash)

  _______                     ________        __
 |       |.-----.-----.-----.|  |  |  |.----.|  |_
 |   -   ||  _  |  -__|     ||  |  |  ||   _||   _|
 |_______||   __|_____|__|__||________||__|  |____|
          |__| W I R E L E S S   F R E E D O M
 -----------------------------------------------------
 OpenWrt 19.07.7, r11306-c4a6851c72
 -----------------------------------------------------
=== WARNING! =====================================
There is no root password defined on this device!
Use the "passwd" command to set up a new password
in order to prevent unauthorized SSH logins.
--------------------------------------------------
```
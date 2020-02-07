# Hackintosh CLOVER for Hasee Z6-SL5 D1

## [中文版](https://github.com/Measureless/Hackintosh_Hasee_Z6-SL5D1/blob/master/%E4%B8%AD%E6%96%87%E8%AF%B4%E6%98%8E.md)

## About this project
- The wireless network adapter is Intel® Dual Band Wireless-AC 3165 which doesn't have macOS driver. I suggest to replace it by Broadcom® BCM94352Z. Used drivers BrcmBluetoothInjector.kext, BrcmFirmwareData.kext and BrcmPatchRAM3.kext. After logging in the system, copy them to /Library/Extensions. Then rebuild the cache by consulting [Broadcom BCM94352z/DW1560驱动新姿势[新方法]](https://blog.daliansky.net/Broadcom-BCM94352z-DW1560-drive-new-posture.html) to slove the problem of Bluetooth failure after waking up.
- [AppleALC](https://github.com/acidanthera/AppleALC/releases) and [Lilu](https://github.com/acidanthera/Lilu/releases) were updated to the newest versions.
- In order to drive the Intel® HD 530 graphics card，used the SSDT-PNLF.aml from [神舟Z6sl5-d1 10.14.1 EFI分享-远景论坛-微软极客社区](http://bbs.pcbeta.com/forum.php?mod=viewthread&tid=1800126). And added "change GFX0 to IGPU" in config.plist.
- Used image [【黑果小兵】macOS Catalina 10.15.3 19D76 正式版 with Clover 5103原版镜像[双EFI版]](https://blog.daliansky.net/macOS-Catalina-10.15.3-19D76-Release-version-with-Clover-5103-original-image-Double-EFI-Version.html) which can be booted normally, but sometimes it maybe stuck at the progress bar. Shut down the laptop by the power botton directly, then reboot after while, it will be normal.
- CLOVER theme used [clover-theme-minimal](https://github.com/al3xtjames/clover-theme-minimal).
- CLOVER version can be updated at [clover-builder](https://github.com/Dids/clover-builder/releases).

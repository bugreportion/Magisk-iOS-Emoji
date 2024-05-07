# [Apple Emoji](https://emojipedia.org/apple)
Systemlessly replaces emoji font with emojis from iOS.  
>
> [!TIP]
> This module can be installed via OverlayFS on Magisk, which permits you to hide the detection of modifications in system and making emoji displaying correct even in apps from which the root is hidden by Magisk Hide. [Read here for more details.](https://github.com/HuskyDG/magic_overlayfs#magisk-overlayfs)

## Changelog
v17.4-1:
- Fixed compatibility issues with KernelSU/APatch *(at least it should be)* by [@dtingley11.](https://github.com/dtingley11)  
To avoid root detections on KSU, use [Zygisk Next](https://github.com/Dr-TSNG/ZygiskNext) module with Enforce Denylist option.
- Fetching updates from GitHub via manager now working.
- Added automatic cleaning of /data/fonts.
- Merged `NotoColorEmoji.ttf` (updated one, which should fix some emoji that were visually smaller than others). [(ed68541)](https://github.com/Keinta15/Magisk-iOS-Emoji/commit/ed6854134ea59ebc7b54e3f625b4115f3dc51794)
- Merged clearing of Gboard cache on install. [(28137f0)](https://github.com/Keinta15/Magisk-iOS-Emoji/commit/28137f0dad32a8066b1705dc6c80cd0a2a01a833)
- No longer need to reinstall the module to apply emojis in Meta apps, for now just reboot device. 
> I can't actually explain why there were two separate versions of modules while we already checking if overlayfs is available using the installation script... So yes, now there's only one.

v17.4:
- [Added iOS 17.4 Emojis (Unicode 15.1).](https://blog.emojipedia.org/ios-17-4-emoji-changelog/)

## Tested devices
[Post on Reddit with user feedback](https://www.reddit.com/r/Magisk/comments/1ca3ip1/news_ios_emojis_174/)

Module was tested personally by me on the following setups:
- Google Pixel 5 on Stock Pixel ROM and crDroid (Android 13/14) with Magisk.
- Google Pixel 4 on Stock Pixel ROM and LineageOS (Android 13/14) with Magisk/KernelSU.
- Xiaomi POCO F5 on HyperOS and AOSPA (Android 14) with KernelSU.
- Xiaomi Mi 11 on crDroid (Android 14) with Magisk.

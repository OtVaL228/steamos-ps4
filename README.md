# SteamOS 3.4.4 for jailbroken PS4
Based on original SteamOS installed from Steam Deck recovery image
Tested on PlayStation 4 Slim CUH-2216A
# Bugs 
1. gamescope session not working. Launch it from KDE Plasma use this guide: https://ps4linux.com/steam-deck-ui-ps4-linux/
2. Sound in gamescope not working but it working in games
3. Sometimes system failed to load due to systemd errors. In this case just reboot
4. ~~Vulkan is broken.~~ Will be fixed in 0.2 release 
# Requirements
Jailbroken PS4

Kernel 5.x or later with working internet and vulkan for gamescope

Any drive with 16GB capacity or better
# Installation
Format your drive as FAT32 and copy bzImage, intramfs.cpio.gz and SteamOS.tar.xz to the root of the USB drive that you just formatted.

Rename SteamOS.tar.xz to the name that initramfs.cpio.gz requires. For example: psxitarch.tar.xz or arch.tar.xz 

Type exec install-psxitarch.sh or whatever initramf.cpio.gz requires and press Enter. The program will install the distro on your USB device. This will take time depending on the drive’s speed.

Once the process has completed, you will be greeted with the console/tty screen. If it doesn’t load automatically, type exec start-psxitarch.sh or resume-boot and press Enter.

After distro is loaded, press CTRL + ALT + F2 and login. user: deck password: deck 

Type steamos-session-select plasma to start KDE Plasma or steamos-session-select plasma-persistent to start and set up KDE Plasma for boot next time 

Press CTRL + ALT + F1 and you will be switch to KDE Plasma
# Screenshots

![Screenshot_20230114_135609](https://user-images.githubusercontent.com/87971581/212470628-6d6d45b8-ee94-4bd8-b369-b95e30b61df8.png)

![Screenshot_20230114_135631](https://user-images.githubusercontent.com/87971581/212470631-ad886108-db64-421d-a517-37250a6ce15d.png)

![Screenshot_20230114_135758](https://user-images.githubusercontent.com/87971581/212470638-eac06800-e3ab-46ca-8592-049364aaf64a.png)

![Screenshot_20230114_135906](https://user-images.githubusercontent.com/87971581/212470646-e26b8b39-a351-4c6e-a2a6-27638df6b330.png)

# NX-StarterPack
A homebrew starter pack & guide for the Nintendo Switch

## What you will need:
* A "first generation" Switch. (Vulnerable to Fusee Gelee / shofEL2)
* A way to put your Switch into RCM [see this guide for more information](https://xghostboyx.github.io/RCM-Guide/)
* A host PC running Windows (Guide may be updated for macOS/Linux/Androud support at a later date)
* A USB 3.0 (usually blue) port on your host pc and a USB-C to A or USB-C to USB-C (if your pc has USB-C)
* An microSD card 2GB or larger, formatted to either FAT32, or exFAT (only if your switch has the exFAT support "update")

## Getting Started:
1. Copy the files in the `sd_root` folder to the root of your Switch's SD Card.
2. Enter RCM mode on your Switch and plug it into your PC.
3. Run `Zadig.exe` with the appropriate permissions.
4. From the device list, choose `APX` (if it's not showing up in the list, go to Options menu and check List All Devices)
5. For the driver type, use the arrows to navigate until you see `libusbK (v3.0.7.0)`
6. Click the big `Install Driver` button. Device Manager should now list `APX` under the `libusbK USB Devices tree item.
7. Depending on your processor type (32-bit or 64-bit), run the relevant `boot_cfw_win*.bat`.
8. Once your Switch boots, you can open the album applet to load the Homebrew Launcher.

## Included Homebrew:
* [2048](https://github.com/BernardoGiordano/2048/), a homebrew port of the popular game of the same name.
* [vgmoose's Homebrew App Store](https://github.com/vgmoose/appstorenx/)
* [Checkpoint](https://github.com/BernardoGiordano/Checkpoint), a save manager for the Nintendo Switch
* [ftpd](https://github.com/WinterMute/ftpd), a tool that can be used to copy and retrieve files from your Switch's microSD card over a local network.
* [sdl_pong](https://github.com/I-EAT-CHEEZE-YO/switch_sdl_pong/), a Pong clone for the Switch.
* [tetrisswitch](https://gbatemp.net/threads/tetriswitch-a-tetris-clone-for-the-switch.498481/#post-7870466), a Tetris clone for the Switch.

## Tools Used:
* [CTCaer's hekate fork](https://github.com/CTCaer/hekate)
* [Pieces of Atmosphere](https://github.com/Atmosphere-NX/Atmosphere)
* [TegraRCMSmash](https://github.com/rajkosto/TegraRcmSmash)



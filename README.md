# NX-Starterpack
A homebrew starter pack & guide for the Nintendo Switch.
This guide will boot you into a "custom firmware" using a combination of the hekate bootloader and Atmosphére CFW. In addition, crash reports are cleared on boot using nx-dreport.
This has only been tested on firmware 5.0.2, but theoretically should work on all firmware versions. (Individual App compatibility may vary).

The files included in this guide work around three of the biggest issues with Switch homebrew:
* Sleep mode works.
* You don't need to reboot after using homebrew to play games.
* Homebrew crashes stay in the crash logs

## What you will need:
* A "first generation" Switch. (Vulnerable to Fusée Gelée / shofEL2)
* A way to put your Switch into RCM [see this guide for more information](https://xghostboyx.github.io/RCM-Guide/)
* A host PC running Windows (Guide may be updated for macOS/Linux/Android support at a later date)
* A USB 3.0 (usually blue) port on your host pc and a USB-C to A or USB-C to USB-C (if your pc has USB-C)
* An microSD card 2GB or larger, formatted to either FAT32, or exFAT (only if your switch has the exFAT support "update")

## Getting Started:
1. Download the zip file of this repo.
2. Copy the files in the `sd_root` folder to the root of your Switch's SD Card.
3. Enter RCM mode on your Switch and plug it into your PC.
4. Run `Zadig.exe` with the appropriate permissions.
5. From the device list, choose `APX` (if it's not showing up in the list, go to Options menu and check List All Devices)
6. For the driver type, use the arrows to navigate until you see `libusbK (v3.0.7.0)`
7. Click the big `Install Driver` button. Device Manager should now list `APX` under the `libusbK USB Devices` tree item.
8. Depending on your processor type (32-bit or 64-bit), run the relevant `boot_cfw_win*.bat`.
9. Once your Switch boots, you can open the album applet to load the Homebrew Launcher.

## Included Homebrew:
* [2048](https://github.com/BernardoGiordano/2048/), a homebrew port of the popular game of the same name.
* [vgmoose's Homebrew App Store](https://github.com/vgmoose/appstorenx/)
* [Checkpoint](https://github.com/BernardoGiordano/Checkpoint), a save manager for the Nintendo Switch
* [ftpd](https://github.com/WinterMute/ftpd), a tool that can be used to copy and retrieve files from your Switch's microSD card over a local network.
* [sdl_pong](https://github.com/I-EAT-CHEEZE-YO/switch_sdl_pong/), a Pong clone for the Switch.
* [tetrisswitch](https://gbatemp.net/threads/tetriswitch-a-tetris-clone-for-the-switch.498481/#post-7870466), a Tetris clone for the Switch.

## Tools Used:
* [CTCaer's hekate fork](https://github.com/CTCaer/hekate)
* [Pieces of Atmosphére](https://github.com/Atmosphere-NX/Atmosphere)
* [TegraRCMSmash](https://github.com/rajkosto/TegraRcmSmash)
* [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu)
* [nx-dreport](https://github.com/Thog/nx-dreport)
* [Zadig](https://github.com/pbatard/libwdi), part of libwdi.

## Credits:
* [ReSwitched](https://reswitched.tech/) for fusée gelée & [libtransistor](https://github.com/reswitched/libtransistor).
* [Switchbrew](https://github.com/switchbrew/) for [nx-hbmenu](https://github.com/switchbrew/nx-hbmenu) & [libnx](https://github.com/switchbrew/libnx).
* [naehrwert](https://github.com/nwert) for [hekate](https://github.com/nwert/hekate).
* [CTCaer](https://github.com/CTCaer/) for their [hekate fork](https://github.com/CTCaer/hekate).
* [SciresM](https://github.com/SciresM), [TuxSH](https://github.com/TuxSH), [hexkyz](https://github.com/hexkyz) and co. for [Atmosphére](https://github.com/Atmosphere-NX/Atmosphere)
* The developers of all the included homebrew.
* [Plailect](https://github.com/Plailect) for inspiring me to write guides.

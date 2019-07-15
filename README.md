# Installing macOS Mojave 10.14.5
==================
## What works?
- BIOS: A26
- Processor: Intel Core Intel® Core™ i7-4600M (All SpeedStep stages).
- Video Card: Intel® HD Graphics 4600 (Work - QE/CI).
- Chipset: Intel I217-LM (Work)
- Mini DisplayPort (No device for test)
- HIMI Port (No device for test)
- VGA AMD Radeon HD 8790 (Not Work)
- Audio: ALC292 (Work)
- WiFi/Bluetooth (Not work). Replaced with DW1550 (BCM94352HMB) (not native - need some kext)
- Ethernet: Intel I217-LM (Work)
- Card Reader (Detect but no device for test)
- Keyboard and ALPS Touchpad (Work)
- Battery (Work)
- Webcam (Work)
- Fingerprint Reader (Not work)
- USB3.0 && USB2.0 (Work)
- Sleep, Restart, Shutdown (Work)
- Airdrop, Handoff, Instant Hotspot and Continuity (Only Work With DW1550 because it have Standard IEEE is 802.11ac and Frequency Range is 5GHz)
## Setup
### Requirements
- One USB flash drive of 8GB or bigger
- macOS Mojave install app (size: 6GB) (use macOS Mojave Patcher to download, sometime you download on AppSotre only have 5-6MB)
- Clover Bootloader in [here](https://sourceforge.net/projects/cloverefiboot/) Recomemed for verison 4961
- Clover custom some part for install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v2.4k-r4961)
- Clover for OS after install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v2.4k-r4961-b)

### Bootable USB Drive
<strong>Note</strong>: Create Bootable USB Drive on macOS device (VWmare or VituralBox)
[Create Bootable USB Drive](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/wiki/Create-Bootable-USB-Drive)

### Bios Settings
Set to Default, apply, then set SATA Operations to AHCI, set Boot List Option to UEFI.

## Install macOS
You Can Do It Yourself
## Post-Installation
Install Clover Bootloader to Drive have OS
Read in [Post Installation](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/wiki/Post-Installation)
## Fix issue
- ...
- for other issue, you can see [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/issues)

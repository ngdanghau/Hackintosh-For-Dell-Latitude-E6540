# Installing macOS Mojave 10.14.5
==================
## What works?
- BIOS: A26
- Processor: Intel Core Intel® Core™ i7-4600M (All SpeedStep stages).
- Video Card: Intel® HD Graphics 4600 <code>Work with QE/CI</code>.
- Chipset: Intel I217-LM <code>Work</code>
- Mini DisplayPort <code>No device for test</code>
- HIMI Port <code>No device for test</code>
- VGA AMD Radeon HD 8790 <code>Not Work</code>
- Audio: ALC292 <code>Work</code>
- WiFi/Bluetooth <code>Not Work</code>. Replaced with DW1550 (BCM94352HMB)  to <code>Work</code>(not native - need some kext)
- Ethernet: Intel I217-LM <code>Work</code>
- Card Reader  <code>No device for test</code>
- Keyboard and ALPS Touchpad <code>Work</code>
- Battery <code>Work</code>
- Webcam <code>Work</code>
- Fingerprint Reader <code>Not Work</code>
- USB3.0 && USB2.0 <code>Work</code>
- Sleep, Restart, Shutdown <code>Work</code>
- Airdrop, Handoff, Instant Hotspot and Continuity <strong>(Only Work With DW1550 because it have Standard IEEE is 802.11ac and Frequency Range is 5GHz)</strong>
## Setup
### Requirements
- One USB flash drive of 8GB or bigger
- macOS Mojave install app (size: 6GB) ([use macOS Mojave Patcher](http://dosdude1.com/mojave/) to download, sometime you download on AppStore only have 5-6MB)
- Clover Bootloader in [here](https://sourceforge.net/projects/cloverefiboot/) Recomemed for verison 4961
- Clover custom some part for install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v2.4k-r4961)
- Clover for OS after install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v2.4k-r4961-b)

### Bootable USB Drive
<strong>Note</strong>: Create Bootable USB Drive on macOS device (VWmare or VituralBox)
[Create Bootable USB Drive](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/wiki/Create-Bootable-USB-Drive)

### Bios Settings
Set to <code>Default</code>, apply, then set <code>SATA Operations</code> to <code>AHCI</code>, set <code>Boot List Option</code> to <code>UEFI</code>.

## Install macOS
You Can Do It Yourself
## Post-Installation
Install Clover Bootloader to Drive have OS
Read in [Post Installation](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/wiki/Post-Installation)
## Fix issue
- ...
- for other issue, you can see [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/issues)

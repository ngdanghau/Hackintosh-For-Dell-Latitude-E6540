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
- Download macOS Mojave install app (size: 6GB) ([use macOS Mojave Patcher](http://dosdude1.com/mojave/) to download, sometime you download on AppStore only have 5-6MB)
- Download Clover Bootloader in [here](https://sourceforge.net/projects/cloverefiboot/) Recomemed for verison 4961
- Clover custom some part for install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v1.0)
- Download Clover for OS after install in [here](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/releases/tag/v2.4k-r4961)

### Bootable USB Drive
<strong>Note</strong>: 
- Create Bootable USB Drive on macOS device (VMware or VituralBox)
- In Clover v2.5k, some foler change name. <code>driver64UEFI</code> to <code>drivers/UEFI</code>
- [Create Bootable USB Drive](https://github.com/ngdanghau/DELL-latitude-E6540-macOS/wiki/Create-Bootable-USB-Drive)
- Adter Create Bootable USB Drive, one Disk with name EFI is show in desktop, open it and go to <code>EFI/CLOVER</code>
- Exact a <code>CloverForInstallOS.zip</code> and open <code>CloverForInstallOS</code> 
- In <code>CloverForInstallOS</code> , you see 1 file config.plist and 3 folder are drivers, kexts and pactched.
- Replace <code>config.plist</code> in <code>EFI/CLOVER</code> with <code>config.plist</code> in <code>CloverForInstallOS</code> 
- Go to <code>EFI/CLOVER/kexts</code> and remove all folder except folder "Other".
- Copy all kext in <code>CloverForInstallOS/kexts</code> to <code>EFI/CLOVER/kexts/Other</code>.
- Go to <code>EFI/CLOVER/ACPI</code> and replace <code>patched</code> folder with <code>patched</code> folder from <code>CloverForInstallOS</code>
- Last, copy file in <code>CloverForInstallOS/drives/HFSPlus.efi</code> to <code>EFI/CLOVER/drivers64UEFI</code>.
![Clover](https://raw.githubusercontent.com/ngdanghau/DELL-latitude-E6540-macOS/master/screenshots/Clover.png)
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

## Credits
- Special Thanks to [Acidanthera](https://github.com/acidanthera) for most of the Kexts.
- Special Thanks to [RehabMan](https://github.com/RehabMan).
- Thanks to [Clover Bootloader](https://sourceforge.net/projects/cloverefiboot/).

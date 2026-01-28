# Planning our next release

Feel free to chime in, add issues and proposals!

## Planning for siduction 2025.2

### General Planning

**Release schedule**
* How many more releases do we want to / can we do in 2025?
  * A snapshot every two months at testbuilds.siduction.org

**New features:**
* Can we add the new Plasma Login Manager standalone or as alternative?
* ~~Add Timeshift to package list~~  
  ~~set it up to do a first image right after install~~ # Rejected
* Calamares, new module Bootmanager selection with a choice of Grub or systemd-boot.
* ~~possibly Limine as bootloader instead of GRUB. It offers a nice tool for Snapper called [limine-snapper-sync](https://gitlab.com/Zesko/limine-snapper-sync), that allows direct booting into any Snapper snapshot directly from the bootloader menu.~~ # Not now, because exclusively with efi. Keep it in here for later
* allow bcachefs through DKMS: [linuxnews.de, 23.09.2025](https://linuxnews.de/bcachefs-via-dkms-in-debian-und-ubuntu/)

**Enhancement:**
* The configuration of XFCE requires our attention.
  * [x] Do not truncate the desktop icon text but wrap it.
  * [x] When the desktop is inactive: Icon text background transparent instead of gray.  
        Refer to: https://github.com/siduction/settings-xfce/issues/5
  * The switch to Weyland may make work easier?
* Insert os-release file
  https://github.com/siduction/release-orga/issues/25
* Revise cli-installer / fll-installer
  + [x] ~~**gdisk** is absolutely essential. It belongs back into the ISOs.~~
    + fdisk (now) supports gpt. Most queries are easier with lsblk and blkid.  
  + [x] Support nvme.
  + [x] Add btrfs support.
  + [x] Add check for internet connection.
  + [x] Add a query from non-free sources.
  + On TTY wrong border and shadow when 'su' is used instead of 'sudo' in the live system.
  + [x] Add Bootmanager selection with a choice of Grub or systemd-boot.

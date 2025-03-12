# Planning our next release

Feel free to chime in, add issues and proposals!

## Planning for siduction 2025.1

### General Planning

**Release schedule**
* How many more releases do we want to / can we do in 2025?
  * A snapshot every two months at testbuilds.siduction.org
* If we want to integrate Timeshift, maybe it's a good idea to do it now.

**New features:**
* Add Timeshift to package list
  * set it up to do a first image right after install
* Calamares, new module Bootmanager selection with a choice of Grub or systemd-boot.

**Enhancement:**
* The configuration of XFCE requires our attention.
  * [x] Do not truncate the desktop icon text but wrap it.
  * [x] When the desktop is inactive: Icon text background transparent instead of gray.  
        Refer to: https://github.com/siduction/settings-xfce/issues/5
  * The switch to Weyland may make work easier?
* APT signatures
  https://github.com/siduction/release-orga/issues/26
* Insert os-release file
  https://github.com/siduction/release-orga/issues/25
* Revise cli installer
  + Grep locales and set it into cli.
  + Add btrfs support.
  + Add Bootmanager selection with a choice of Grub or systemd-boot.

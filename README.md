# ThinkPad T430 EFI for macOS Catalina 10.15.1

This is a repo which includes files required to run macOS Catalina 10.15.1 on a ThinkPad T430 (2349U2B) with Intel HD 4000 graphics and a 1600x900 display.

These are the versions of software included in this repository:

* Clover r5098
* [AppleSupportPkg](https://github.com/acidanthera/AppleSupportPkg/releases) 2.0.9, 2.1.2
* [Lilu](https://github.com/acidanthera/Lilu/releases) 1.3.9
* [WhateverGreen](https://github.com/acidanthera/WhateverGreen/releases) 1.3.4
* [AppleALC](https://github.com/acidanthera/AppleALC/releases) 1.4.3
* [HibernationFixup](https://github.com/acidanthera/HibernationFixup/releases) 1.3.0
* [IntelMausi](https://github.com/acidanthera/IntelMausi/releases) 1.0.2


## Important info

* Don't put any kexts in S/L/E, Clover will load them automatically. If you have some already, delete them and rebuild your cache before rebooting.

* If you have a model with the 1366x768 display, make sure to set `ig-platform-id` in `config.boot` to `0x01660003`.

* Don't forget to generate your own SMBIOS values!

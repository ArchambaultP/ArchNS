# ArchNS
Script to compile Netsurf 3.8(Dev) for AmigaOS 3.9 on Arch Linux,
Modified and updated version of [NetScript](http://www.github.com/DNADNL/NetScript "NetScript")

## Info

The script uses gcc to compile Netsurf 3.8 (The most recent development version) for AmigaOS 3.9. It was written with Arch Linux in mind, but should work with most other distros provided you have the pre-required packages.

## Content Of This Repository
* ArchNS.sh: The script to compile Netsurf onto your machine
* libs:
** mpc-0.8.2.tar.gz: Backup of the mpc package v.0.8.2 that could be found at multiprecision.org/mpc/ (Site Down), it is used by the toolchain so we have to use this one instead of the online version
** autoconf2.64-2.64-1-any.pkg.tar.xz: Arch compatible package to install the autoconf2.64 binary. This is not installed automatically and is provided for troubleshooting purposes.

## How to use NetScript(ArchNS) ?
1. Clone this repository onto your machine
2. cd into ArchNS
3. bash ArchNS.sh (make sure to have super user rights)

If everything went smoothly you should find a .tar of your compiled netsurf version. Simply extract this .tar to a drive readable by your Amiga machine and install it in your amiga machine.

## Troubleshooting
### Having problems with autoconf2.64 during the toolchain compilation ?
Go to the ArchNS/libs directory and manually install autoconf2.64-2.64-1-any.pkg.tar.xz

If you use pacman, run the command: pacman -U autoconf2.64-2.64-1-any.pkg.tar.xz, note that this package is untracked.

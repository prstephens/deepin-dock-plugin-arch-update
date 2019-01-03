Arch Linux Updates Indicator DDE Dock Plugin
===============
Update indicator for Arch Linux and Deepin Dock, 

Depend on `pacman-contrib`

Install
--------

### AUR ###
[deepin-plugin-arch-update](https://aur.archlinux.org/packages/deepin-dock-plugin-arch-update/)

### Binary ###
Download from [Releases](../../releases/) the `libarch_update.so` file and copy it (as sudo) to 
`/usr/lib/dde-dock/plugins/`

### Compile it locally ###
Require Qt

```
mkdir build
cd build
qmake ../source
make
sudo make install
pkill dde-dock
```

TODO
-------
- [X] non-blocking dialog
- [ ] translation (waiting for API)
- [ ] show update version infos
- [ ] add travis.ci support (can I)

Other notes
-------
Not sure if it's a bug of Qt or not, but if I name qrc file `icons.qrc`, it will not be able to find the resource files. 
It will be appreciated if anyone can help me with why. 

Credits
----------
All icons are based on Thayer Williams' Archer logo, winner of Arch Linux logo contest.

Some portions are inspired by 
[arch-update](https://github.com/RaphaelRochet/arch-update), 
[Deepin official plugins](https://github.com/linuxdeepin/dde-dock/tree/master/plugins) 
and [CMDU](https://github.com/sonichy/CMDU_DDE_DOCK)

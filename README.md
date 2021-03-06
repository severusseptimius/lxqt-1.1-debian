# lxqt-1.1-debian

This repo contains .deb packages of LXQt 1.1 that are tested with Debian unstable/testing and Ubuntu 22.04.
It is structured in three main folders: 
- **lxqt** (this is the one you probably want as a normal user)
- **lxqt-dev** (this one contains the development versions of the packages; unless you need them to build lxqt from source you don't need them)
- **lxqt-dbgsym** (this one contains the debugging packages. Unless you really need them, you *shouldn't* have to install them.)

# Installing

**Packages for arm64 can be found [here](https://github.com/djsftree/arm64_playground_djsftree/tree/1.1.0-packages), thanks to [@djsftree](https://github.com/djsftree)**

### FOR UBUNTU
If you want to install these packages on *ubuntu, it is strongly recommended that you use this PPA:
https://launchpad.net/~severusseptimius/+archive/ubuntu/lxqt
***

### FOR DEBIAN
Before installing, it is recomended that you do `sudo apt remove libfm-qt*`, followed by `apt --fix-broken install`. This will remove the packages that might make problems, but it will not remove your configuration files.
After that, just 
```
git clone https://github.com/severusseptimius/lxqt-1.1-debian   # assuming you didn't do this already
cd lxqt-1.1-debian
cd lxqt
sudo apt install ./*.deb
sudo reboot
...
Enjoy!
```

# Reporting bugs

All bugs related to packaging can be reported here. Before starting a new issue, make sure that it is in fact a packaging bug and not an upstream one.
Upstream bugs should be reported here: https://github.com/lxqt/

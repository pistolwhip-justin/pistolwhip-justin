# How to install XDM on any Linux distribution

subhra74 edited this page on Mar 19, 2020 · [1 revision](https://github.com/subhra74/xdm/wiki/How-to-install-XDM-on-any-Linux-distribution/_history)

# Installation of XDM on any linux distribution.

[](https://github.com/subhra74/xdm/wiki/How-to-install-XDM-on-any-Linux-distribution#installation-of-xdm-on-any-linux-distribution)

If you have any outdated version installed already, please remove them completely. Also remove any directory named xdman under /opt ( open terminal and type rm -rf /opt/xdman and restart your computer )

Installation steps:

- Download the installation archive from: [https://github.com/subhra74/xdm](https://github.com/subhra74/xdm)
- Lets asume you have downloaded the file in your download folder. (~/Downloads) ( make sure the file name after download is xdm-setup-7.2.10.tar.xz, not xdm-setup-7.2.10.tar(1).xz etc )
- Open terminal and switch to the directory using cd ~/Downloads
- Now type tar xvf xdm-setup-7.2.10.tar.xz
- Threre should a file named install.sh created inside the folder now
- Now you will need to be root user to start installation ( use sudo if you are using ubuntu/debian/mint/solus/elementary etc, and su -C for SUSE, manjaro, fedora etc )
- Type sudo ./install.sh or su -C ./install.sh
- After installation is done then start XDM from start menu.

# Uninstall

[](https://github.com/subhra74/xdm/wiki/How-to-install-XDM-on-any-Linux-distribution#uninstall)

sudo /opt/xdman/uninstall.sh

###
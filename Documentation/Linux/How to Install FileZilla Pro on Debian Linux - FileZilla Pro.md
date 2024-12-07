---
title: "How to Install FileZilla Pro on Debian Linux - FileZilla Pro"
source: "https://filezillapro.com/docs/v3/basic-usage-instructions/install-filezilla-pro-on-debian-linux/"
author:
  - "[[FileZilla Pro]]"
published: 2019-10-22
created: 2024-12-06
description: "FileZilla Pro - How to Install FileZilla Pro on Debian Linux"
tags:
  - "clippings"
---
> This feature is only available on FileZilla Pro, if you didn’t buy it yet you can [buy FileZilla Pro from our Store](https://store.filezillapro.com/order/checkout.php?PRODS=5654472&CLEAN_CART=ALL&SHORT_FORM=1&DESIGN_TYPE=2&QTY=1&CART=1&CARD=2&ORDERSTYLE=nLWw5JXfqnQ=).

Follow the steps below to install FileZilla Pro on Debian Linux.

1. Go to the directory where the installation file was downloaded.  
This file is named *FileZilla\_Pro\_\_x86\_64-linux-gnu.tar.bz*.
2. Open the file using the extract tool.
3. Extract the files to the destination directory.
4. Go to the directory where the files were extracted.
5. Go to `FileZilla3 directory`.
6. Start the program using the **filezilla** executable in the `bin/` subdirectory.

**Launch from command line**

If it fails to launch from the file manager you may need to launch from the command line.  
See below how to install and launch from command line:

1. Open a terminal.
2. Change to the directory where the installation file was downloaded,for example:  
cd ~/Downloads/
3. Extract the file with:

tar xf FileZilla\_Pro\_*\_x86\_64-linux-gnu.tar.bz*
4. Launch FileZilla Pro with:  
`FileZilla3/bin/filezilla`

### To create a icon on the desktop:

1. Copy the `FileZilla3/share/applications/filezilla.desktop `to your Desktop directory.  
cp FileZilla3/share/applications/filezilla.desktop $HOME/Desktop
2. Open the file `filezilla.desktop` in a text editor. Adjust the paths at **Exec** and **Icon**  
according to the directory where the installation file was extracted to.**Exec** is the path to the FileZilla Pro executable file. For example:

`Exec=/opt/FileZilla3/bin/filezilla   Icon=/opt/FileZilla3/share/icons/hicolor/scalable/apps/filezilla_pro.svg`

- A shortcut icon is shown on the desktop.
- Right-click the shortcut and choose **Allow launching**.
- The shortcut now shows the FileZilla Pro icon:

## ![](https://filezillapro.com/wp-content/uploads/2019/10/Screenshot_debianLinux_shortcut.png)

- If you use another desktop environment, like KDE, you need to change the shortcut properties to allow execution:

- Right click the shortcut.
- Choose Properties.
- Mark **Is Executable** or **Allow executing file as program**.

**Make it available in the list of applications**

Note that some desktop environments do not support desktop icons. In this case move the `filezilla.desktop `to your *applications* directory:

`mv filezillapro.desktop ~/.local/share/applications`

The shortcut will be in the list of available applications.

**Supported distributions**

Please note that due to differences in distributions, the provided binaries for Debian Linux might not work on different GNU/Linux systems.

The systems where FileZilla Pro is known to work are:

- Debian 10.4 or greater
- Fedora 31 or greater
- CentOS 8.1 or greater
- Ubuntu 20.04 or greater
- Linux Mint 20 or greater
- openSUSE Leap 15.3 or greater
- Red Hat Enterprise Linux 8.1 or greater
- Rocky Linux 9
- Arch Linux

The following distributions where FileZilla Pro does not work:

- Ubuntu 18.04
- openSUSE Leap 15.1 and openSUSE Leap 15.2
- Linux Mint 19.3

Version 3.66;5 checked on February 7th, 2024 confirmed to work with the following versions:

- Debian 12.4
- Mint 21.1
- Ubuntu 23.10
- Fedora 39, installation of libxcrypt-compat package is required with the command below  
`sudo dnf install libxcrypt-compat`
- openSUSE Leap 15.5
- Red Hat Enterprise Linux 9, installation of GTK+ 2 package is required with the command below  
`sudo dnf install gtk2`
- Rocky 9, installation of GTK+2 package is required with the command below  
`sudo dnf install gtk2`
- Arch Linux: installation of GTK+2 and libxcrypt-compat packages is required with the command below  
`sudo pacman -S gtk2 libxcrypt-compat`

Tags: [Debian Linux](https://filezillapro.com/docs/v3/tag/debian-linux/), [Debian Linux Installation](https://filezillapro.com/docs/v3/tag/debian-linux-installation/), [FileZilla Debian](https://filezillapro.com/docs/v3/tag/filezilla-debian/), [FileZilla Pro Debian](https://filezillapro.com/docs/v3/tag/filezilla-pro-debian/), [FileZilla Pro Debian Linux installation](https://filezillapro.com/docs/v3/tag/filezilla-pro-debian-linux-installation/)
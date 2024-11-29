---
title: "Install and Use Ventoy on Ubuntu [Complete Guide]"
source: "https://itsfoss.com/use-ventoy/"
author:
  - "[[Sagar Sharma]]"
published: 2023-07-26
created: 2024-11-27
description: "Get started with installing and using Ventoy with our guide that covers everything from live Linux USB to bootable Windows USB."
tags:
  - "clippings"
---
[![Warp Terminal](https://itsfoss.com/assets/images/warp-terminal.webp)](https://www.warp.dev/?utm_source=its_foss&utm_medium=display&utm_campaign=linux_launch)

Being a distro hopper, I can relate to the pain of having one ISO image on a flash drive. But not anymore!

If you [constantly distro hop](https://itsfoss.com/distrohopping-issues/), or you just want to carry multiple ISO files in a single pen drive, there is a solution - **Ventoy**.

In this guide, I'll walk you through the following:

- **Installing Ventoy on Linux**
- **Creating a live Linux USB**
- **Booting from Ventoy**
- **Using multiple Linux distros on a single USB**
- **Creating Windows bootable USB**
- **Using Linux and Window on a single USB**

So let's start with the first one.

Ventoy is not available in the default repositories or 3rd party repos on Ubuntu. But, it is available on AUR for Arch users. This simply means you cannot [use apt to install the package](https://itsfoss.com/apt-command-guide/).

So in this case, we have to install Ventoy from source. Fret not, you just need to follow along the steps below, it is easy.

📋

****You can use this method for any Linux distribution****.

**1**. Visit the [official download page of Ventoy](https://www.ventoy.net/en/download.html) and choose the file ending with `linux.tar.gz`:

![download the latest version of Ventoy in Ubuntu](https://itsfoss.com/content/images/2023/07/download-the-latest-version-of-Ventoy-in-Ubuntu.png)

**2**. Now, open your terminal and [use the cd command](https://itsfoss.com/cd-command/) to navigate to where the Ventoy file was downloaded. For most users, it will be the `Downloads` directory:

```
cd Downloads
```

The Ventoy binaries are shipped in the form of the tarball and to untar (or extract) the package, you can [use the tar command](https://learnubuntu.com/untar-files/) as shown:

```
tar -xzvf ventoy-*.tar.gz
```

**3**. Once extracted, you will find a directory of Ventoy. Use the cd command to get into that directory.

In my case, it was `ventoy-1.0.93`, so I will be using the following:

```
cd ventoy-1.0.93
```

If you list the directory contents, you will find that there are multiple scripts:

```
ls
```
![use ls command to list the directory contents](https://itsfoss.com/content/images/2023/07/use-ls-command-to-list-the-directory-contents.png)

But what you need is `VentoyWeb.sh` which allows you to flash your drive using your browser without any commands.

**4**. To execute the script, use the following command:

```
sudo ./VentoyWeb.sh
```
![start the ventoy web script in terminal](https://itsfoss.com/content/images/2023/07/start-the-ventoy-web-script-in-terminal.png)

As you can see, it started the Ventoy server and to access it, copy the given URL and paste it to the address bar of your browser.

Once you do that, it will look like this:

![start ventoy web in browser to install Ventoy in Ubuntu](https://itsfoss.com/content/images/2023/07/start-ventoy-web-in-browser-to-install-Ventoy-in-Ubuntu.png)

By default, it will be enabled to work with the secure boot option and this is the reason it shows the 🔒 (lock) symbol with the version name.

I do not recommend you change this setting, but if you would like to, you can disable this option from the **Option→Secure boot Support**:

![enable or disable secure boot option in Ventoy](https://itsfoss.com/content/images/2023/07/enable-or-disable-secure-boot-option-in-Ventoy.png)

Once done, select the storage path on which you want to install Ventoy and hit the `Install` button.

Before installing, it will ask you to check the drive two times as it will format the drive, so make sure to take a backup of critical data (if there's any):

![Ventoy warning before installing in Ubuntu](https://itsfoss.com/content/images/2023/07/Ventory-warning-before-installing-in-Ubuntu.png)

Click to enlarge the image

Once done, you will see a message—"*Ventoy has been successfully installed to the device*":

![Ventoy has been successfully installed to the device in Ubuntu](https://itsfoss.com/content/images/2023/07/Ventoy-has-been-successfully-installed-to-the-device-in-Ubuntu.png)

And the installation is done.

## Create a Live USB with Ventoy

To create a Live USB with Ventoy, first, you need to download an ISO image of your preferred operating system.

While Ventoy should support almost everything, I would still recommend checking the compatibility from [their official page](https://www.ventoy.net/en/compatible.html).

To make the USB bootable with Ventoy, all you have to do is paste the ISO file to the Ventoy drive. Yes, it is as simple as that! 🤯

![](https://itsfoss.com/content/images/2023/07/make-bootable-USB-using-ventoy-1.gif)

📋

If you want to check the hash of the ISO file for file integrity, you can find the steps mentioned below.

### Using GtkHash to check the hash (optional)

While Ventoy does can check the hash, it can only be used when you boot with Ventoy and most users won't have another system to compare the hash.

So it is a good idea to check the hash sum on a working system.

To [check the hash](https://itsfoss.com/checksum-tools-guide-linux/), I would recommend using **GtkHash** which is a simple GUI tool that lets you check the hash for the files.

It is available as a Flatpak so if you haven't enabled flatpak, then, you can refer to our detailed guide on [using Flatpak on Linux](https://itsfoss.com/flatpak-guide/). Your software center may include support for it, so you might want to check that too.

Once setup, you can use the following command to install it on your system:

```
flatpak install flathub org.gtkhash.gtkhash
```

After installation, start **GtkHash** from your system menu and follow two simple steps to check the hash value:

First, select the ISO file:

![Select an ISO file to check the hash sum](https://itsfoss.com/content/images/2023/07/Select-an-ISO-file-to-check-hash.png)

Click to enlarge the image

And paste the hash from the website you got the ISO file in the `Check` field, then press the `Hash` button:

![](https://itsfoss.com/content/images/2023/07/check-hash-for-ISO-file-to-create-bootable-drive-in-ventoy.png)

Click to enlarge the image

As you can see, it shows a green signal 🟢 meaning, the hash matched!

## Boot Using Ventoy USB Drive

Before I walk you through the boot process, there are two modes that you should consider if the ISO doesn't boot.

- `GRUB2`: If any of your Linux distros doesn't boot, you may enable the `GRUB2` mode by pressing `Ctrl + r`. **Remember, it will only work with distros having a grub2 config file.**
- `WIMBOOT`: If you run into problems while booting Windows ISO, you can enable the wimboot mode by pressing `Ctrl + w`.

📋

You should only be using any of the given modes if the default settings do not work for you.

While you can reboot your system and press **F12, del, F2,** or other respective keys to get into the BIOS, you can also choose to use the terminal if you like.

To get into the BIOS of your system while using Linux, all you have to do is use the following command in your terminal:

```
systemctl reboot --firmware-setup
```

If you want to boot from Ventoy every time you start your system with the flash drive, head to the boot menu and change the boot priorities with Ventoy's USB drive as the first.

If not, you can simply use the boot menu every time and select to boot from it Ventoy manually (overriding the defaults).

![Change boot order in BIOS](https://itsfoss.com/content/images/2023/07/Change-boot-order-in-BIOS-1.jpg)

Now, save changes and exit from the BIOS (as per your preferences), and you will see a Ventoy screen with one or multiple distros:

![](https://itsfoss.com/content/images/2023/07/Ventoy-boot-screen.png)

Here's how it looks like with multiple distros onboard:

![use multiple distros in one pendrive using ventoy in Ubuntu linux](https://itsfoss.com/content/images/2023/07/use-multiple-ISO-in-Ventoy.png)

You can use the arrow keys to navigate through the multiple options.

And if you choose the Linux distro as I did, then by pressing the enter key on the distro option, you will see the following options:

![Boot options for Linux in ventoy](https://itsfoss.com/content/images/2023/07/Boot-options-in-Ventoy.png)

Boot from the normal mode (selected by default); if it doesn't work, you can boot from the grub2.

![](https://public-files.gumroad.com/akcz661m3xkpsztskivjmh2agj22)

## Create a Windows bootable USB

The process for [creating a bootable Windows USB](https://itsfoss.com/bootable-windows-usb-linux/) remains the same, but this time, you have to copy the Windows ISO file to the Ventoy drive. But let me walk you through it so that you can avoid any confusion.

![create bootable drive of Windows using Ventoy on Ubuntu Linux](https://itsfoss.com/content/images/2023/07/Create-Windows-bootable-drive-with-ventoy.gif)

So, now if you will boot from Ventoy, you will see a Windows ISO file. I went with Windows 10, so mine looks like this:

![](https://itsfoss.com/content/images/2023/07/Create-bootable-drive-of-Windows-using-Ventoy.png)

Once you press enter, you will see a little different boot menu compared to what it displayed with Linux distros on the flash drive:

![Booting up Windows from Ventoy in Linux](https://itsfoss.com/content/images/2023/07/Booting-up-Windows-from-Ventoy-in-Linux.png)

If you notice carefully, it added `Boot in wimboot mode` an option.

First, try with the normal mode and if it does not work, use the wimboot mode.

![](https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png)

## Use multiple Linux distros in a single USB

To [use the multiple distros on a single USB](https://itsfoss.com/multiple-linux-one-usb/), all you have to do is copy multiple ISO files in the Ventoy disk drive:

![use multiple distros in Ventoy](https://itsfoss.com/content/images/2023/07/Use-multiple-distros-in-Ventoy.gif)

Yes. It's that simple. Want more details? This detailed article will help you with that.

![](https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png)

## Use Linux and Windows ISOs in the same USB

By far this is the most realistic implementation where you can boot from Windows and your favorite Linux distros.

The method remains the same. All you have to do is copy the Windows ISO and Linux ISO to Ventoy.

Here, I have copied the ISO of LinuxMint and Windows, but you can do more as per the drive size:

![](https://itsfoss.com/content/images/2023/08/Copy-Linux-and-Windows-ISO-to-Ventoy.gif)

Once done, you boot from Ventoy and you'd see ISO of Windows ISO and Linux:

![Boot from Windows and Linux ISOs in Ventoy](https://itsfoss.com/content/images/2023/08/Boot-from-Windows-and-Linux-ISOs-in-Ventoy.png)

And there you have it!

## Wrapping Up

I've been using Ventoy for the past two years and I can't recall any situation where it backfired! It works like a charm. Some people, like my colleague Ankush, prefer [Etcher for creating live USBs](https://itsfoss.com/install-etcher-linux/). That too is a good tool but I prefer Ventoy.

![](https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png)

But I'm curious to know how you utilize Ventoy and your experiences 🤔

*💬 Don't forget to share your thoughts in the comments box below.*
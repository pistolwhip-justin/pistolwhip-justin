---
aliases:
  - "Flatpak for Beginners: An Introduction to Downloading Software With Flatpak"
---
# Flatpak for Beginners: An Introduction to Downloading Software With Flatpak

![4](https://static1.makeuseofimages.com/wordpress%2Fwp-content%2Fauthors%2F60e335f2cfe88-199678826_10160618037302079_5955514759433243364_n.jpg?fit=crop&w=90&h=90)

By [Wini Bhalla](https://www.makeuseof.com/author/wini-bhalla/)

Published Jun 25, 2021

Follow

Share

Link copied to clipboard

[Linux](https://www.makeuseof.com/tag/linux/ "Linux")

### Related

[

![Screen of a phone with passwords, padlocks, and keys around it.](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/10/screen-of-a-phone-with-passwords-padlocks-and-keys-around-it.jpg)





](https://www.makeuseof.com/popular-passwords-list-123456/)

##### [This List of Popular Passwords Shows We Still Don’t Understand Online Security](https://www.makeuseof.com/popular-passwords-list-123456/ "This List of Popular Passwords Shows We Still Don’t Understand Online Security")

[

![A Pixelbook Go Chromebook on a table in the garden](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/08/chromebook-in-garden-featured-1.jpg)





](https://www.makeuseof.com/chromebook-next-laptop-reasons-why/)

##### [6 Reasons Why Your Next Laptop Should Be a Chromebook](https://www.makeuseof.com/chromebook-next-laptop-reasons-why/ "6 Reasons Why Your Next Laptop Should Be a Chromebook")

[

![Keyboard with the at sign implying email addresses](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/11/keyboard-with-the-at-sign-implying-email-addresses.jpg)





](https://www.makeuseof.com/signs-its-time-to-get-a-new-email-address/)

##### [9 Signs It’s Time to Get a New Email Address](https://www.makeuseof.com/signs-its-time-to-get-a-new-email-address/ "9 Signs It’s Time to Get a New Email Address")

Sign in to your MUO account

![getting started with flatpak](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2021/06/introduction-to-flatpak.jpg)

Linux newbies are in for a treat since they can install packages while saving time and effort. Canonical, Ubuntu's parent company, was the first to implement snaps, a cross-distribution dependency-free software.

With Snap came Flatpak, another universal packaging system, written in C. Considered a package management utility, it allows a user to install and run applications in an isolated environment.

## Basic Terminologies

Like Snap, Flatpak aims at simplifying software management across Linux distributions. Here are some common terminologies worth knowing:

- **Flatpak**: This is a system used for building, distributing, and running sandboxed desktop applications on Linux.
- **Runtime**: Runtimes are also called platforms as these work as integrated platforms to provide basic utilities needed for a Flatpak application to work.
- **Flatpak application**: These are applications a user can install using the **flatpak** command on their computer.

## Advantages of Using Flatpak

- **Universality**: Flatpak, as a utility service manager, allows a user to install and run applications virtually on almost any Linux desktop. This will include any non-GNU distributions, read-only operating systems, systemd-free distributions, or other architectures.
- **Innovation friendly**: Flatpak promotes distribution maintainers to help developers focus on their innovation goals.
- **Stability**: Any breakages within an application don’t cause the system to break. This is because Flatpak runtimes are contained and don’t interfere with the system’s working.
- **Rootless install**: You don’t need elevated privileges when installing a Flatpak application/runtime.
- **Sandboxed applications**: One of Flatpak’s primary goals is to improve system security by isolating applications from one another. Applications are sandboxed and run in separate silos.

Related:[A Beginners Guide to Software Repositories in Ubuntu](https://www.makeuseof.com/ubuntu-software-repositories-introduction/)

## Installing Flatpak on Linux Distributions

There are different ways to install Flatpak, depending on the Linux distro you use.

Flatpak installation is a two-step procedure. The first step includes installing Flatpak via a package manager. The second step comprises adding Flatpak’s repository Flathub, from where you can install various applications.

Here’s how you can install the package on different Linux distros:

### On Ubuntu and Mint

By default, Flatpak supports Ubuntu 18.04, Mint 19.3, and their later versions. You can install the package on Ubuntu and Linux Mint using APT:

```
sudo apt install flatpak
```

### On Debian and Debian-Based Distros

To install Flatpak on Debian based distros like Elementary and Zorin, you need to add a PPA to your system before downloading the package:

```
sudo add-apt-repository ppa:alexlarsson/flatpaksudo apt updatesudo apt install flatpak
```

You can also use the commands mentioned above to install Flatpak on Ubuntu.

### On Red Hat and Fedora

To install on RHEL-based distributions like Fedora and CentOS, run this command:

```
sudo dnf install flatpak
```

Alternatively, you can also use the YUM package manager:

```
sudo yum install flatpak
```

### On OpenSUSE

Issue the following command to install Flatpak on OpenSUSE:

```
sudo zypper install flatpak
```

### On ArchLinux/Manjaro

Last but not least, to install the package on Arch Linux and its derived distributions, run the following command:

```
sudo pacman -S flatpak
```

Related:[Flathub vs. Snap Store: The Best Sites for Downloading Linux Apps](https://www.makeuseof.com/tag/flathub-vs-snap-store-linux-apps/)

## Adding the Flathub Repository in Linux

The next step is to add Flatpak’s repository, Flathub, so that you can download and install applications from one of its most popular and widely used repositories.

To [add the repository on Linux](https://www.makeuseof.com/how-to-manually-add-linux-software-repositories/), run this command:

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

## How to Use Flatpak on Linux

Using Flatpak is quite similar to using other package managers on Linux. You can search for and install applications from the Flathub repository using the Flatpak command-line tool.

### Search Applications on Flathub

Before jumping in to install the applications, you can check if a certain application is available within the repository. The default format for this command is:

```
flatpak search application-name
```

As an example, let’s search for Spotify and install it if it is available.

```
flatpak search spotify
```

The resulting values will display the application ID, version, branch, and remotes along with a description of the software.

### Install Packages Using Flatpak

The basic syntax to install applications using Flatpak is:

```
flatpak install remotes applicationID
```

For example, to install Spotify, you can use:

```
flatpak install flathub com.spotify.Client
```

### Launch an Application

Use the following command format to launch an application:

```
flatpak run applicationID
```

For example:

```
flatpak run com.spotify.Client
```

This will eventually launch the Spotify application on your system.

### List Installed Flatpak Packages

Let’s take this a step further. To get a list of all the Flatpak packages installed on your system:

```
flatpak list
```

### Update Installed Packages

To update Flatpak packages within your system, run:

```
flatpak update
```

If all packages are already up to date, there will be no new changes after running the aforementioned command.

### Uninstall Software Using Flatpak

If you have installed an application and no longer want to retain it, you can successfully uninstall it using the **uninstall** method. The default syntax of the command is:

```
flatpak uninstall applicationID
```

Since we have just installed Spotify, try uninstalling the application by typing:

```
flatpak uninstall com.spotify.Client
```

## Enabling the GNOME Repository

Just like Flathub, the GNOME repository contains all GNOME core applications. The central repository itself has two versions: stable and nightly.

### Add the GNOME Stable Repository

Use **wget** to download the GPG keys for the repository:

```
wget https://sdk.gnome.org/keys/gnome-sdk.gpg
```

Add the GNOME Flatpak repository to your system using **remote-add**:

```
sudo flatpak remote-add --gpg-import=gnome-sdk.gpg --if-not-exists gnome-apps https://sdk.gnome.org/repo-apps/
```

To install the nightly version instead, issue the following commands:

```
wget https://sdk.gnome.org/nightly/keys/nightly.gpgsudo flatpak remote-add --gpg-import=nightly.gpg --if-not-exists gnome-nightly-apps https://sdk.gnome.org/nightly/repo-apps/
```

### Listing Remote Repositories

To list all configured remote repositories:

```
flatpak remotes
```

The above command will list the repositories you have added to your system. It will also display if the repository is a system-wide installation or specific to a few users only.

### Deleting A Flatpak Repository

The basic syntax to delete a repository is:

```
sudo flatpak remote-delete remote-name
```

...where **remote-name** is the name of the remote repository.

For example, to remove the Flathub repository from your system:

```
sudo flatpak remote-delete flathub
```

### Repairing Flatpak Installation

Use the **repair** command to repair the Flatpak installation on your system:

```
sudo flatpak repair
```

The command takes a little time to run, so be patient and wait for it to execute fully.

### Kill a Flatpak Process

To kill any Flatpak process, first, check which processes are running:

```
sudo flatpak ps
```

To kill a process:

```
sudo flatpak kill applicationID
```

To check if the system killed the process successfully:

```
sudo flatpak ps
```

Related:[How to Display Process Related Information on Linux Using the ps Command](https://www.makeuseof.com/ps-command-linux/)

## Making the Most Out of Flatpak’s Commands

As a beginner, you will probably feel overwhelmed by the different terminologies, jargon, and tons of commands available within Linux distros. However, Flatpak is here to make your life easier by letting you install applications safely and securely.

If you are just starting, it is best to explore the various functionalities slowly and steadily as you go about understanding the different nuances available within the distros. If you don't want to deal with the command line at all, consider switching to Snap and Snap Store to install packages on Linux.

- [  
    ](https://www.makeuseof.com/category/linux/ "Linux")
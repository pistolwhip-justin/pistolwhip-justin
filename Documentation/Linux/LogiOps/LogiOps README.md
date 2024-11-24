# LogiOps

[](https://github.com/PixlOne/logiops/blob/main/README.md#logiops)

sudo systemctl restart logid

[![Build Status](https://github.com/PixlOne/logiops/actions/workflows/build-test.yml/badge.svg)](https://github.com/PixlOne/logiops/actions/workflows/build-test.yml/badge.svg)

This is an unofficial driver for Logitech mice and keyboard.

This is currently only compatible with HID++ >2.0 devices.

## Configuration

[](https://github.com/PixlOne/logiops/blob/main/README.md#configuration)

[Refer to the wiki for details.](https://github.com/PixlOne/logiops/wiki/Configuration)

You may also refer to [logid.example.cfg](https://github.com/PixlOne/logiops/blob/main/logid.example.cfg) for an example.

Default location for the configuration file is /etc/logid.cfg, but another can be specified using the `-c` flag.

## Dependencies

[](https://github.com/PixlOne/logiops/blob/main/README.md#dependencies)

This project requires a C++20 compiler, `cmake`, `libevdev`, `libudev`, `glib`, and `libconfig`. For popular distributions, I've included commands below.

**Arch Linux:** `sudo pacman -S base-devel cmake libevdev libconfig systemd-libs glib2`

**Debian/Ubuntu:** `sudo apt install build-essential cmake pkg-config libevdev-dev libudev-dev libconfig++-dev libglib2.0-dev`

**Fedora:** `sudo dnf install cmake libevdev-devel systemd-devel libconfig-devel gcc-c++ glib2-devel`

**Gentoo Linux:** `sudo emerge dev-libs/libconfig dev-libs/libevdev dev-libs/glib dev-util/cmake virtual/libudev`

**Solus:** `sudo eopkg install cmake libevdev-devel libconfig-devel libgudev-devel glib2-devel`

**openSUSE:** `sudo zypper install cmake libevdev-devel systemd-devel libconfig-devel gcc-c++ libconfig++-devel libudev-devel glib2-devel`

## Building

[](https://github.com/PixlOne/logiops/blob/main/README.md#building)

To build this project, run:

```shell
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make
```

To install, run `sudo make install` after building. You can set the daemon to start at boot by running `sudo systemctl enable logid` or `sudo systemctl enable --now logid` if you want to enable and start the daemon.

## Development

[](https://github.com/PixlOne/logiops/blob/main/README.md#development)

The project may only run as root, but for development purposes, you may find it convenient to run as non-root on the user bus. You must compile with the CMake flag `-DUSE_USER_BUS=ON` to use the user bus.

## Donate

[](https://github.com/PixlOne/logiops/blob/main/README.md#donate)

This program is (and will always be) provided free of charge. If you would like to support the development of this project by donating, you can donate to my Ko-Fi below.

[![Buy Me a Coffee at ko-fi.com](https://camo.githubusercontent.com/7ed30defb0d001964cbb2b5def4fbf3466179d3868823d77e5958f6a3b76f639/68747470733a2f2f63646e2e6b6f2d66692e636f6d2f63646e2f6b6f6669312e706e673f763d32)](https://ko-fi.com/R6R81QQ9M)

I'm also looking for contributors to help in my project; feel free to submit a pull request or e-mail me if you would like to contribute.

## Compatible Devices

[](https://github.com/PixlOne/logiops/blob/main/README.md#compatible-devices)

[For a list of tested devices, check TESTED.md](https://github.com/PixlOne/logiops/blob/main/TESTED.md)

## Credits

[](https://github.com/PixlOne/logiops/blob/main/README.md#credits)

Logitech, Logi, and their logos are trademarks or registered trademarks of Logitech Europe S.A. and/or its affiliates in the United States and/or other countries. This software is an independent product that is not endorsed or created by Logitech.

Thanks to the following people for contributing to this repository.

- [Clément Vuchener & contributors for creating the old HID++ library](https://github.com/cvuchener/hidpp)
- [Developers of Solaar for providing information on HID++](https://github.com/pwr-Solaar/Solaar)
- [Nestor Lopez Casado for providing Logitech documentation on the HID++ protocol](http://drive.google.com/folderview?id=0BxbRzx7vEV7eWmgwazJ3NUFfQ28)
- Everyone listed in the contributors page
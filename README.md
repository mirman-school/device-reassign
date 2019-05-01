# device-reassign
Reassign Devices with a single command

For use with macOS devices.

## Installation

```bash
git clone https://github.com/mirman-school/device-reassign
cd device-reassign
chmod 755 device-reassign
sudo cp device-reassign /usr/local/
```

## Installation with Munki

This file comes with a script to build install/uninstall packages using [munkipkg](https://github.com/munki/munki-pkg). Have it installed and in your `$PATH`.

The script will create a folder for the install package. Version is based on the value in the `version` file. Change it as you need to.

```bash
git clone https://github.com/mirman-school/device-reassign
cd device-reassign
chmod 755 ./build
./build
munkiimport device-reassign-install/build/device-reassign-"$(cat version)".pkg
```



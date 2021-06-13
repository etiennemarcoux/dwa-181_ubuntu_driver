# DWA-181, AC1300 Driver installation on ubuntu 18.04

First install dependencies depending on your package manager this can be done on Debian/Ubuntu using apt:

```
sudo apt update && sudo apt upgrade
sudo apt install build-essential
```
Download the Linux driver file from D-Link Technical Support:
https://support.dlink.com/ProductInfo.aspx?m=DWA-181-US


Next unzip the downloaded folder, and unzip the file in there.
There should be a folder called driver with a driver tarball, with the name rtl88x2BU_WiFi_linux_v5.8.7.1_*.tar.gz

Decompress in whatever fashion you see fit, open the newly decompressed folder and open a terminal to this location.

```
sudo make
sudo make install
sudo modprobe DWA_181
```
Credits: https://askubuntu.com/a/1272531

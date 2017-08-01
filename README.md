# TogoTelekom

Linux TogoTelekom USB Stick connection configuration repo with a short description of usage.

## Installation

### What you need to install
*   `wvdial` Debian (`sudo apt-get install wvdial`) CentOS (`yum install wvdial`) FreeBSD (Build from source)
*   `usb_modeswitch` [Source Code Website](http://www.draisberghof.de/usb_modeswitch/#download)
*   *   Debian (`sudo apt-get install usb-modeswitch`) CentOS (`yum install usb-modeswitch`)
*   `lsusb` to find your current and after usb_modeswitch Hardware ID, Manufactor ID. (Debian/CentOS) has it build-in.
*   `pppd` to initial the actually connection, usually will be installed with `wvdial`. If not Debian (`sudo apt-get install pppd`) CentOS (`yum install pppd`)

### Configuration files
The `wvdial.conf` should be in `/etc/` and from the `usb_modeswitch.d/19d2:0016` in `/etc/usb_modeswitch.d/` folder. After you have copied the files in the belong folder, edit the `wvdial.conf` (Important) with your Username, Password and PIN if nescessary.

### Test connection
I'm using `screen` to keep the connections up and running, for testing you can keep a simple terminal open.
The simplest way to test the connection is to start `wvdial`. I've added PIN and modem-start what it does, take a look below.

### Advanced Configuration
In wvdial.conf you can add the PIN (If you haven't yet disabled, I suggest to disable it). To activate it just hit `wvdial pin`.
The another tab is "EVDO" what you may know from TogoTelekom connection manager. Usually PPP is connecting with the regular mode, who you probably don't want. The trick `wvdial modem-start` who is activating the "high-speed"

## Meta

[![License](https://img.shields.io/github/license/SHelfinger/TogoTelekom.svg?colorB=00aeef)](https://opensource.org/licenses/GPLv3)
[![Repository size](https://reposs.herokuapp.com/?path=shelfinger/TogoTelekom&color=00aeef)](https://github.com/SHelfinger/TogoTelekom)
[![Website](https://img.shields.io/badge/website-shelfinger.eu-00aeef.svg)](https://shelfinger.eu/)
[![Status](https://img.shields.io/badge/status-testing-blue.svg)](https://github.com/SHelfinger/TogoTelekom)
[![GitHub forks](https://img.shields.io/github/forks/badges/shields.svg?style=social&label=Fork)](https://github.com/SHelfinger/TogoTelekom/fork)

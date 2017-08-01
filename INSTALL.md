## Debian
Update the repos
`sudo apt-get update`
Install the required programs
`sudo apt-get install ppp wvdial usb-modeswitch`
If usb-modeswitch didn't install (Not found), please check the [source website](http://www.draisberghof.de/usb_modeswitch/#download)

## CentOS
Install the required programs
`yum install ppp wvdial usb-modeswitch`
If usb-modeswitch didn't install (Not found), please check the [source website](http://www.draisberghof.de/usb_modeswitch/#download)

## Configuration
Download [wvdial.conf](etc/wvdial.conf) and [19d2:0016](usb_modeswitch.d/19d2:0016) and add it in the belong folder /etc/wvdial.conf and /etc/usb_modeswitch.d/19d2:0016

## Test Connection
`wvdial`
If failed let us know

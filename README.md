# roseapple-pi-snappy-image
This repo is to provide the snappy image for Roseapple-Pi.

We use Ubuntu 15.04 and stable channel as our snappy target.
There's package (a.k.a snap) list in snappy:  
```bash
(RoseapplePi)ubuntu@localhost:~$ snappy list
Name         Date       Version      Developer 
ubuntu-core  2015-11-13 10           ubuntu    
webdm        2015-11-23 0.9.4        canonical 
roseapple-pi 2015-11-23 IGKJeJGLLDKH sideload  
```

In snappy, the default user account is:  
user:ubuntu
password:ubuntu

## Flash to SD card

```bash
xzcat ${image} | pv | sudo dd of=/dev/${device} bs=32M ; sync
```

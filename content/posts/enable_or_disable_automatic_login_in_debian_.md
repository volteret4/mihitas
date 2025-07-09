+++
title = "Automatic login in Linux"
date = "2025-07-09"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "volteret4"
cover = ""
tags = ["tags: ArchLinux"]
keywords = ["tags: ArchLinux"]
description = "Autologin Linux"
showFullContent = false
readingTime = true
hideComments = false
draft = false
+++

> [ORIGEN](https://linux.how2shout.com/enable-or-disable-automatic-login-in-debian-11-bullseye/)

`sudo nano /etc/lightdm/lightdm.conf`

Scroll to the end of the file, add:

`autologin-user=username`

`sudo nano /etc/sddm.conf.d/autologin.conf`

```ini fold title:example_title
[Autologin]
User=john
Session=kodi # xfce, plasma, ...
```

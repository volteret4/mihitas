+++
title = "Enable_or_disable_automatic_login_in_debian_"
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

> <a href="https://linux.how2shout.com/enable-or-disable-automatic-login-in-debian-11-bullseye/" class="tc-tiddlylink-external" rel="noopener noreferrer" target="_blank">https://linux.how2shout.com/enable-or-disable-automatic-login-in-debian-11-bullseye/</a>

`sudo nano /etc/lightdm/lightdm.conf`

Scroll to the end of the file, add:

`autologin-user=username`

`sudo nano /etc/sddm.conf.d/autologin.conf`

```ini fold title:example_title
[Autologin]
User=john
Session=kodi # xfce, plasma, ...
```

+++
title = "Wakeonlan Pa Siempre"
date = "2026-01-18"
author = "volteret4"
cover = ""
tags = ["lan", "systemd"]
keywords = ["lan", "systemd"]
description = "Manten persistencia en al configuración de wakeonlan"
showFullContent = false
readingTime = true
hideComments = false
+++


> <a href="https://serverfault.com/questions/1082356/how-to-make-wake-on-lan-persistent-in-debian-buster" class="tc-tiddlylink-external" rel="noopener noreferrer" target="_blank">https://serverfault.com/questions/1082356/how-to-make-wake-on-lan-persistent-in-debian-buster</a>

Primero modifica la BIOS para que permita WOL
 
Segundo comprueba que tu tarjeta de red sea capaz de WOL;
 
`sudo ethtool eth0`
 
```sh
Supports Wake-on: pumbg
Wake-on: d
```

Actívalo:

`sudo ethtool -s eth0 wol g`

Comprueba que funcione, y para hacerlo permanente has de crear un servicio de `systemd`:

Luego crea este servicio para mantener persistencia:

```sh

$ cat /etc/systemd/system/wol.service
[Unit]
Description=Configure Wake-up on LAN

[Service]
Type=oneshot
ExecStart=/sbin/ethtool -s eth0 wol g

[Install]
WantedBy=basic.target
```

Por ultimo actíva el servicio con `system-ctl`:

`sudo systemctl enable wol.service`

`sudo systemctl daemon-reload`

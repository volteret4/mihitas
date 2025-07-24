+++
title = "Eliminar Clave De Known_hosts"
date = "2025-07-24"
author = "volteret4"
cover = ""
tags = [""linux", "ssh", "known_hosts""]
keywords = [""linux", "ssh", "known_hosts""]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++


Para eliminar las claves que referencien a dietpi:
```sh
   ssh-keygen -f "/home/$USER/.ssh/known_hosts" -R "dietpi"

+++
title = "Eliminar Clave De Known_hosts"
date = "2025-07-09"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = "Eliminar clave de un servidor"
showFullContent = true
readingTime = true
hideComments = false
+++

Para eliminar las claves que referencien a dietpi:

```
   ssh-keygen -f "/home/$USER/.ssh/known_hosts" -R "dietpi"
```

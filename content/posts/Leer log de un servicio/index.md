+++
title = "Leer Log De Un Servicio"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = []
keywords = []
description = "Flags útiles para usar con journalctl"
showFullContent = false
readingTime = true
hideComments = false
+++


> [Origen](https://unix.stackexchange.com/questions/475292/how-to-watch-output-from-systemd-service)

```sh
journalctl -f -u mystuff.service
```

 `-f, --follow`
Mostrar solo las entradas de diario más recientes e imprimir continuamente las nuevas entradas a medida que se añaden al diario.


 `-u, --unit=UNIT|PATTERN`

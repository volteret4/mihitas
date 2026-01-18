+++
title = "Copiar Archivo De Un Contenedor De Proxmox"
date = "2026-01-18"
author = "volteret4"
cover = ""
tags = ["archivos", "commands", "shell"]
keywords = ["archivos", "commands", "shell"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


Con este commando puedes copiar un archivo a tu host
```sh
pct pull <vmid> <path> <destination>

# por ejemplo
pct pull 135 /root/contenedores/pollo.zip pollo.zip
```


+++
title = "Watch"
date = "2026-01-20"
author = "volteret4"
cover = ""
tags = ["oneline", "shell"]
keywords = ["oneline", "shell"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


Gracias a esta app puedes vigilar el output de una tarea repetitiva.

```bash
watch ls -alh . # mostrará el contenido de la carpeta actual,, actualizando cada dos segundos
watch --differences df -h # mostrará el uso de los discos casi en tiempo real
watch --chgexit lsbl # Saldrá del comando al detectar un cambio
```



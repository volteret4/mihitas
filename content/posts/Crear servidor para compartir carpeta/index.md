+++
title = "Crear Servidor Para Compartir Carpeta"
date = "2025-07-10"
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = "Descarga archivos de tu servidor rápidamente"
showFullContent = true
readingTime = true
hideComments = false
+++

Crea un servidor http en una carpeta para poder descargar archivos rápidamente

```sh
python3 -m http.server 8000 --bind 0.0.0.0 --directory /ruta/al/directorio
```

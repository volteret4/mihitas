+++
title = "Archivos Modificados Recientemente"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["Esto"]
keywords = ["Esto"]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++


```bash
# Muestra archivos modificados en el último día
find /ruta/a/tu/directorio -type f -mtime -1

#Esto listará los archivos con detalles como permisos, propietario, tamaño y fecha de modificación.
find /ruta/a/tu/directorio -type f -mmin -60 -ls  
```




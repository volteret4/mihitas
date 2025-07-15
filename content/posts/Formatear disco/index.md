+++
title = "Formatear Disco"
date = "2025-07-15"
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


## Formatear disco

``` bash
# Crear nueva tabla de particiones 
sudo fdisk /dev/sdXY
	# Orden: g, n, w

# Formatear disco
mkfs [options] [-t type fs-options] device [size]

	sudo mkfs -t ext4 /dev/sdb1  # EJEMPLO
```

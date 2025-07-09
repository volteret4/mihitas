+++
title = "Crear ISO De Dispositivo"
date = "2025-07-10"
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = "Copia tus unidades fisicas en una ISO."
showFullContent = true
readingTime = true
hideComments = false
+++


Crea una imagen de una unidad como un disco duro o una tarjeta de memoria.

``` bash
sudo dd if=/dev/sdX of=name-of-iso.iso status="progress"

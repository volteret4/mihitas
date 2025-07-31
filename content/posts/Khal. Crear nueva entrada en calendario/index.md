+++
title = "Khal. Crear Nueva Entrada En Calendario"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = []
keywords = []
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++


Usa khal para agregar una entrada en el calendario.

Reemplaza las variables del siguiente commando por tus datos.

```sh
khal new -a discos "${fecha}":::"${title}"

zenity –info –text='creado nuevo evento'
```

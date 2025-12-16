+++
title = "Se Insultado Al Fallar Contraseña De Sudo"
date = "2025-12-16"
author = "volteret4"
cover = ""
tags = ["oneline", "sudo"]
keywords = ["oneline", "sudo"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


Primero edita las opciones de sudo con `sudo visudo` y añade la línea:
```bash
Defaults insults
```

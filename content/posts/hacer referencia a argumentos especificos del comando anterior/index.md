+++
title = "Hacer Referencia A Argumentos Especificos Del Comando Anterior"
date = "2026-01-17"
author = "volteret4"
cover = ""
tags = ["shell"]
keywords = ["shell"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


Puedes usar `!:#` para referenciar segmentos del commando anterior
```sh
touch archivo.txt
echo !:1 
archivo.txt

touch 1.txt 2.txt
echo !:2
2.txt
```

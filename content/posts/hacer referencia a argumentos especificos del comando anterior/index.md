+++
title = "Hacer Referencia A Argumentos Especificos Del Comando Anterior"
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

> Origen: ChatGPT

También puedes hacer referencia a argumentos específicos del comando anterior utilizando la sintaxis !:n, donde "n" es el número del argumento que deseas utilizar. Por ejemplo, si el comando anterior fue ls -l archivo.txt, puedes utilizar la siguiente sintaxis para imprimir el nombre del archivo:

```
echo !:2
```

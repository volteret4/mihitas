+++
title = "Git. Retroceder En Github"
date = "2025-07-22"
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = "Restaurar commit"
showFullContent = true
readingTime = true
hideComments = false
+++



```sh
 git restore archivo1 archivo2
```

Si además de restaurarlos quieres deshacer cualquier cambio que hayas _staged_ con `git add`, usa:

```sh
 git restore --staged archivo1 archivo2 git restore archivo1 archivo2

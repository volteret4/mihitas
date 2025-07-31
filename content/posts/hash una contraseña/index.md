+++
title = "Hash Una Contraseña"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["linux", "python", "contraseña", "hash"]
keywords = ["linux", "python", "contraseña", "hash"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


El `PASSWORD_HASH` lo puedes generar con:

```python
import hashlib 
print(hashlib.md5("TU_CONTRASEÑA".encode()).hexdigest())
```

O pasándole un argumento

```python
import hashlib 
import sys
print(hashlib.md5(sys.argv[0].encode()).hexdigest())

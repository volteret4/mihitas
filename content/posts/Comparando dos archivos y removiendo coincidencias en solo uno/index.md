+++
title = "Comparando Dos Archivos Y Removiendo Coincidencias En Solo Uno"
date = "2025-07-15"
author = "volteret4"
cover = ""
tags = ["compare", "file", "linux", "grep"]
keywords = ["grep", "linux", "compare", "file"]
description = "Problemas con firma PGP y pacman"
showFullContent = false
readingTime = true
hideComments = false
+++

> [Origen](<https://stackoverflow.com/questions/37503186/comparing-two-files-by-lines-and-removing-duplicates-from-first-file" class="tc-tiddlylink-external>)

Remove lines from test1 because they are in test2:

```bash
grep -vxFf test2 test1
```

To overwrite test1:

```bash
grep -vxFf test2 test1 >test1.tmp && mv test1.tmp test1
```

+++
title = "Mount NTFS"
date = "2025-07-15"
author = "volteret4"
cover = ""
tags = [""]
keywords = [""]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++


## Instalar
```bash
sudo apt install fuse
sudo apt install ntfs-3g
```
## Montar
```bash
sudo mount -t ntfs /dev/sdXy /path
```

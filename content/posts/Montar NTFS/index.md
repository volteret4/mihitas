+++
title = "Montar Ntfs"
date = "2026-01-17"
author = "volteret4"
cover = ""
tags = ["filesystems"]
keywords = ["filesystems"]
description = ""
showFullContent = false
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

+++
title = "Comando Para Copiar A Exfat"
date = "2025-07-15"
author = "volteret4"
cover = ""
tags = ["exfat"]
keywords = ["exfat"]
description = "Maneja unidades compatibles con windows"
showFullContent = true
readingTime = true
hideComments = false
+++

### Montar

```sh
sudo mount -t exfat -o uid=1000,gid=1000,umask=022 /source /dest
```

### Copiar

```sh
rsync -avh --info=progress2 --no-perms --no-owner --no-group --ignore-existing --exclude='temp/*' /mnt/dietpi_userdata/NFS/2TB/moode/ /mnt/500GB/Musica/
```

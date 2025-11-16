+++
title = "Instalar Steam En Archlinux"
date = "2025-11-16"
author = "volteret4"
cover = ""
tags = ["pacman", "steam"]
keywords = ["pacman", "steam"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


Edit la configuración de `pacman`
```shell
% vim /etc/pacman.conf
```

Elimina el comentario de la sección `[multilib]`

```shell
#[multilib]
#Include = /etc/pacman.d/mirrorlist
```

Quedando asi

```shell
[multilib]
Include = /etc/pacman.d/mirrorlist
```

Guarda el archivo y actualiza

```shell
% pacman -Syyu
```

Ya puedes instalar Steam:

```shell
% pacman -S steam
```
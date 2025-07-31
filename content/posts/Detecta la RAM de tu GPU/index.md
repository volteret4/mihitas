+++
title = "Detecta La RAM De Tu GPU"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["Arch", "Linux", "gpu-passtrough", "gpu", "video"]
keywords = ["Arch", "Linux", "gpu-passtrough", "gpu", "video"]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++




> [Origen](https://www.cyberciti.biz/faq/howto-find-linux-vga-video-card-ram)


```sh
glxinfo | grep -E -i 'device|memory'
```

Ea, a merendar.

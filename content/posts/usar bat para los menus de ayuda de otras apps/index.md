+++
title = "Usar Bat Para Los Menus De Ayuda De Otras Apps"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["linux", "bat", "ayuda", "alias"]
keywords = ["linux", "bat", "ayuda", "alias"]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++

Añade esto a tu `.zshrc`

```zsh
 alias -g -- -h='-h 2>&1 | bat --language=help --style=plain'
 alias -g -- --help='--help 2>&1 | bat --language=help --style=plain'
```

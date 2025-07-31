+++
title = "Kopia Server Add User"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["linux", "kopia", "server", "user"]
keywords = ["linux", "kopia", "server", "user"]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++


Añade un nuevo usuario así desde el servidor, reemplazando el texto entre llaves:

```docker
 docker exec {kopia_container_name} kopia server user add {user}@{hostname}
```


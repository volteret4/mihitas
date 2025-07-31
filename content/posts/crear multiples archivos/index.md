+++
title = "Crear Multiples Archivos"
date = "2025-07-31"
author = "volteret4"
cover = ""
tags = ["linux", "touch", "multiple", "files", "oneline"]
keywords = ["linux", "touch", "multiple", "files", "oneline"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++


```bash {1} ❴lineos="true"❵ 
touch roles/system/tasks/{essential,main,user,ssh}.yml

tree roles
roles
└── system
    └── tasks
        ├── essential.yml
        ├── main.yml
        ├── ssh.yml
        └── user.yml

3 directories, 4 files
```


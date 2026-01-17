+++
title = "Rsync Evitar Directorio"
date = "2026-01-17"
author = "volteret4"
cover = ""
tags = ["rsync"]
keywords = ["rsync"]
description = ""
showFullContent = false
readingTime = true
hideComments = false
+++



## [Exclude a Specific Directory](https://linuxize.com/post/how-to-exclude-files-and-directories-with-rsync/#exclude-a-specific-directory)

```sh
rsync -a --exclude 'dir1' src_directory/ dst_directory/
```
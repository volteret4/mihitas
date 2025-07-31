+++
title = "Fail2ban How To Unban Ips That Are Blocked"
date = "2025-07-24"
author = "volteret4"
cover = ""
tags = ["Fail2ban", "linux"]
keywords = ["Fail2ban", "linux", "unban", "ip"]
description = "Permite ips con fail2ban"
showFullContent = true
readingTime = true
hideComments = false
+++

> **[Origen](https://bobcares.com/blog/fail2ban-unban-ip/)**

```sh
fail2ban-client set yourjailname unbanip youripaddress
```

+++
title = "Atuin. Historial Del Terminal Con Superpodéres"
date = "2025-07-24"
author = "volteret4"
cover = ""
tags = [ "linux", "atuin", "terminal", "historial", "sync" ]
keywords = [ "atuin","historial" ]
description = ""
showFullContent = true
readingTime = true
hideComments = false
+++

```zsh {lineNos="true" wrap="true" title="Instalar atuin"}
# Instalación
pacman -S atuin
# Añadir añ inicio con zsh
echo 'eval "$(atuin init zsh)"' >> ~/.zshrc
# Importar historial antiugo para zsh
atuin import zsh
# añadir servidor al config
vim `~/.config/atuin/config.toml`
# descomentar linea
sync_addres: http://192.168.1.133:8778      # adaptar
# registrar cuenta
atuin account register  # añadir credenciales nuevas
#guardar llave
atuin key
# sincronizar
atuin sync
```

```sh
services:
  atuin:
    restart: always
    image: ghcr.io/atuinsh/atuin:18.6.1
    command: server start
    volumes:
      - "/home/pepe/contenedores/atuin/config:/config"
    links:
      - postgresql:db
    ports:
      - 8778:8888
    environment:
      ATUIN_HOST: "0.0.0.0"
      ATUIN_OPEN_REGISTRATION: "true"
      ATUIN_DB_URI: postgres://$ATUIN_DB_USERNAME:$ATUIN_DB_PASSWORD@db/$ATUIN_DB_NAME
      RUST_LOG: info,atuin_server=debug
  postgresql:
    image: postgres:14
    restart: unless-stopped
    volumes: # Don't remove permanent storage for index database files!
      - "/home/pepe/contenedores/atuin/database:/var/lib/postgresql/data/"
    environment:
      POSTGRES_USER: ${ATUIN_DB_USERNAME}
      POSTGRES_PASSWORD: ${ATUIN_DB_PASSWORD}
      POSTGRES_DB: ${ATUIN_DB_NAME}


  backup:
    container_name: atuin_db_dumper
    image: prodrigestivill/postgres-backup-local
    env_file:
      - .env
    environment:
      POSTGRES_HOST: postgresql
      POSTGRES_DB: ${ATUIN_DB_NAME}
      POSTGRES_USER: ${ATUIN_DB_USERNAME}
      POSTGRES_PASSWORD: ${ATUIN_DB_PASSWORD}
      SCHEDULE: "@daily"
      BACKUP_DIR: /db_dumps
    volumes:
	  - /home/pepe/contenedores/db_dumps:/db_dumps
    depends_on:
      - postgresql
```

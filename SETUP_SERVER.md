# Setup Zabbix server

## Pre-requisites

- Setup [Docker](https://www.docker.com) trên host server

## Setup server

- Clone project: `https://github.com/zabbix/zabbix-docker.git`
- Config các port liên quan, vd: `ZABBIX_WEB_NGINX_HTTPS_PORT`, `ZABBIX_WEB_NGINX_HTTP_PORT`
- Chạy docker compose với file tương ứng:

  ```bash
  docker compose -f ./docker-compose_v3_alpine_pgsql_latest.yaml up --build --remove-orphan
  ```

## (Optional) Setup reverse proxy với nginx

- Clone và làm theo hướng dẫn `https://github.com/fm39hz/nginx-reverse-proxy-temlate.git`

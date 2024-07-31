# Zabbix active agents with docker-compose

## Pre-requisites

- Setup [Docker](https://www.docker.com) trên host server
- Mở port 10051 trên zabbix server

## Setup monitor host

- Tạo host mới bằng nút `Create new host`
- Nhập host name, ở phần template chọn template `Linux by zabbix agent active`
- Chọn update

## Install agent

- Clone project: `git clone https://github.com/fm39hz/zabbix-active-agent.git`
- Setup environment variables: `cp .env.example .env`:
  - _ZBX_HOSTNAME_: tên host ở trên
  - _ZBX_SERVER_HOST_: ip của zabbix server
  - _ZBX_PASSIVE_SERVER_: domain của server, dùng khi sử dụng passive check

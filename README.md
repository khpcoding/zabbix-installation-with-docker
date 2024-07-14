# Zabbix Docker Deployment

This repository contains a Docker Compose setup for deploying Zabbix version 6 with a MySQL database backend. The setup includes the Zabbix server, Zabbix web frontend, Zabbix agent, and a MySQL database.

## Services

- **db**: MySQL database for Zabbix.
- **zabbix-server**: Zabbix server.
- **zabbix-web**: Zabbix web frontend using Nginx.
- **zabbix-agent**: Zabbix agent.

## Prerequisites

- Docker installed on your local machine.
- Docker Compose installed on your local machine.

## Getting Started

1. Clone this repository:

```sh
git clone https://github.com/yourusername/zabbix-docker.git
cd zabbix-docker
```

## RUN Project 
```
docker-compose up -d
```

## Default Login Credentials
Username: Admin
Password: zabbix

## Configuration
Time Zone: Adjust the PHP_TZ environment variable in the zabbix-web service in the docker-compose.yml file to your preferred time zone.

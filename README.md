# Wordpress

## Description

This is a simple NGINX-Wordpress-MySQL web server.

## Components

* NGINX
* Wordpress
* MySQL

## Installation

### Prerequisite

* [Docker](https://docs.docker.com/engine/install/)
* [Docker Compose](https://docs.docker.com/compose/install/) _(optional, but makes life easier)_

### Build & Run

1. Clone this repository

2. Create an `.env` with all necessary variables.

```bash
# FQDN host name
NGINX_HOST=blog.example.com

# Password to log in to DB
DB_PASS=secrets

# User with privileged access to DB_NAME db
DB_USER=wordpress-admin

# Db which can be access with above credentials.
DB_NAME=wordpress
```

3. Start project.

```bash
docker-compose up -d
```

### Usage

After stack is up, go to https://$hostname:443 to install Wordpress to server. 

Project is installed at [blog.phuongmphan.com](https://blog.phuongmphan.com).

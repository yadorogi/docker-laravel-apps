# Laravel environment on Docker 🐳 and templates for web applications 

![License](https://img.shields.io/github/license/ucan-lab/docker-laravel?color=f05340)
![Stars](https://img.shields.io/github/stars/ucan-lab/docker-laravel?color=f05340)
![Issues](https://img.shields.io/github/issues/ucan-lab/docker-laravel?color=f05340)
![Forks](https://img.shields.io/github/forks/ucan-lab/docker-laravel?color=f05340)

## Introduction

Build a simple laravel development environment with docker-compose.

## Usage

```bash
$ git clone git@github.com:yadorogi/docker-laravel-apps.git
$ cd docker-laravel-apps
$ make create-project # Install the latest Laravel project
$ make install-recommend-packages # Optional
```

http://localhost

## Tips

- Read this [Makefile](https://github.com/yadorogi/docker-laravel-apps/blob/main/Makefile).
- Read this [Wiki](https://github.com/yadorogi/docker-laravel-apps/wiki).

## Container structures

```bash
├── app
├── web
└── db
```

### app container

- Base image
  - [ucan-lab/docker-laravel](https://github.com/ucan-lab/docker-laravel)
  - [php](https://hub.docker.com/_/php):8.0-fpm-buster
  - [composer](https://hub.docker.com/_/composer):2.0

### web container

- Base image
  - [ucan-lab/docker-laravel](https://github.com/ucan-lab/docker-laravel)
  - [nginx](https://hub.docker.com/_/nginx):1.20-alpine
  - [node](https://hub.docker.com/_/node):16-alpine

### db container

- Base image
  - [ucan-lab/docker-laravel](https://github.com/ucan-lab/docker-laravel)
  - [mysql/mysql-server](https://hub.docker.com/r/mysql/mysql-server):8.0

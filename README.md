# Magento Docker components

## Installation
* Install [Docker](https://www.docker.com/get-started)
* Install [Docker-sync](http://docker-sync.io)

### Code

Clone your code into `services/magento` and `services/msi` folders. In result, your folder structure should be next:

```
- services
-- magento
--- magento2ce
--- magento2ee
--msi
--- magento2ce
```

## Configs

1. Copy global config `cp global.env.dist global.env`
1. Copy composer config `cp composer.env.dist composer.env`

## Auth

1. Replace default GitHub token in file `composer.env` with your personal

## Usage

1. Run `docker-sync-stack start` to start sync and up containers
1. Run `docker-compose run cli magento-installer` to install first instance
1. Open `localhost:8080` in your browser for first instance
1. Run `docker-compose run cli-msi magento-installer` to install second instance
1. Open `localhost:8081` in your browser for second instance

## End of work

1. Press `Ctrl + C` to stop Docker till next run

## Nuke environment

1. Run `docker-sync-stack clean` to remove containers

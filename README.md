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

* Copy global config `cp global.env.dist global.env`
* Copy composer config `cp composer.env.dist composer.env`

## Usage

* Run `docker-sync-stack start` to start sync and up containers
* Run `docker-compose run cli magento-installer` to install Magento
* Open `localhost:8080` in your browser for first instance
* Open `localhost:8081` in your browser for second instance

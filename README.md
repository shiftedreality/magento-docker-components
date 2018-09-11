# Magento Docker components

## Installation
* Install [Docker](https://www.docker.com/get-started)
* Install [Docker-sync](https://github.com/EugenMayer/docker-sync)

### Code

Clone your code into `services/magento` and `services/msi` folders. In result you structure should be next:

```
- services
-- magento
--- magento2ce
--- magento2ee
--msi
```

## Usage

* Run `docker-sync-stack start` to start sync and `docker-compose up`
* Run `docker-compose run cli magento-command setup:install --backend-frontname="admin" --cleanup-database --db-host="db" --db-name="magento" --db-user="root" --db-password="magento2" --base-url="http://localhost:8080/" --admin-user="admin" --admin-password="123123q" --admin-email="oposyniak@magento.com" --admin-firstname="Oleh" --admin-lastname="Posyniak"` to install Magento
* Open `localhost:8080` in your browser

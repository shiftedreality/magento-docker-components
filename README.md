# Magento Docker components

## Installation
### Docker-sync

Install https://github.com/EugenMayer/docker-sync for your system

### Code

Clone your code into `services/magento` and `services/msi` folders. In result you structure should be next:

```
- services
-- magento
--- magento2ce
--- magento2ee
--msi
--- magento2ce
```

## Usage

Run `docker-sync-stack start` to start sync and `docker-compose up`

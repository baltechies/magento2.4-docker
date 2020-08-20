![Magento 2](https://cdn.rawgit.com/rafaelstz/magento2-snippets-visualstudio/master/images/icon.png)

#  Magento 2 Docker to Development

### Apache 2.4 + PHP 7.4 + Mysql8 + N98 Magerun 2 + XDebug + ElasticSearch

### Requirements

**MacOS:**

Install [Docker](https://docs.docker.com/docker-for-mac/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose) and [Docker-sync](https://github.com/EugenMayer/docker-sync/wiki/docker-sync-on-OSX).

**Windows:**

Install [Docker](https://docs.docker.com/docker-for-windows/install/), [Docker-compose](https://docs.docker.com/compose/install/#install-compose) and [Docker-sync](https://github.com/EugenMayer/docker-sync/wiki/docker-sync-on-Windows).

**Linux:**

Install [Docker](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/) and [Docker-compose](https://docs.docker.com/compose/install/#install-compose).

### How to use

Clone this repo at your machine.

Create an empty directory src inside cloned repo.

Download magento2.4 source code into src directory. [https://devdocs.magento.com/guides/v2.4/install-gde/composer.html](https://devdocs.magento.com/guides/v2.4/install-gde/composer.html).


Run docker compose command from current repo.
```
docker-compose up -d
```

Now execute magento commands from docker container. If your apache container name is magento24_apache_1, then command would be like. 
```
docker exec -it magento24_apache_1 bash
```

Now install magento2 using Magento2 commands

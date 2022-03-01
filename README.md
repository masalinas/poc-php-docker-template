# Symfony 6 docker containers

A Proof-of-concept of a running Symfony 6 application inside containers

More information from [martinpham Sample](https://dev.to/martinpham/symfony-5-development-with-docker-4hj8)

Clone the project

```shell
git clone https://github.com/masalinas/poc-php-docker-template.git

```

Generate Symfony sources

```shell
cd poc-php-docker-template

symfony new src --webapp
```

Deploy docker compose

```
cd docker

docker-compose up
```

## Compose

### Database (MariaDB)

...

### PHP (PHP-FPM)

Composer is included

```
docker-compose run php-fpm composer
```

To run fixtures

```
docker-compose run php-fpm bin/console doctrine:fixtures:load
```

### Webserver (Nginx)

...

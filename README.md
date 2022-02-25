# Symfony 5 docker containers

A Proof-of-concept of a running Symfony 5 application inside containers

```
git clone https://github.com/masalinas/poc-php-docker-template.git

cd poc-php-docker-template

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

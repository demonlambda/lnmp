FROM php:7.2.24-fpm-alpine3.10

RUN curl -L -o /tmp/redis.tar.gz https://github.com/phpredis/phpredis/archive/5.0.2.tar.gz \
    && tar xfz /tmp/redis.tar.gz \
    && rm -r /tmp/redis.tar.gz \
    && mkdir -p /usr/src/php/ext \
    && mv phpredis-5.0.2 /usr/src/php/ext/redis \
    && docker-php-ext-install pdo_mysql opcache redis \
    && rm -rf /usr/src/php
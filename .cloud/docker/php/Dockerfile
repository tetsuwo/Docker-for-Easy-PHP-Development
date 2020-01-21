FROM php:7.3.7-fpm

# install composer
RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer
RUN apt-get update \
    && apt-get install -y \
    git \
    zip \
    unzip \
    vim \
    cron

RUN apt-get update \
    && apt-get install -y \
    && docker-php-ext-install pdo_mysql

WORKDIR /var/www/html

FROM php:7.1-fpm

# System dependencies
RUN apt-get update
RUN apt-get install -y libicu-dev g++

# PHP Extensions
RUN docker-php-ext-install intl
RUN docker-php-ext-enable opcache

# Set recommended PHP.ini settings
# See https://secure.php.net/manual/en/opcache.installation.php
RUN { \
        echo 'opcache.memory_consumption=128'; \
        echo 'opcache.interned_strings_buffer=8'; \
        echo 'opcache.max_accelerated_files=4000'; \
        echo 'opcache.revalidate_freq=60'; \
        echo 'opcache.fast_shutdown=1'; \
        echo 'opcache.enable_cli=1'; \
    } > /usr/local/etc/php/conf.d/opcache-recommended.ini

WORKDIR /var/vhosts/frontend.i-mscp.net

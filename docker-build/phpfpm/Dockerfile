FROM php:7-fpm

COPY php-fpm.conf /usr/local/etc/php-fpm.conf
COPY pool.d /usr/local/etc/php/pool.d/

#For installing additional php extensions
#RUN docker-php-ext-install -j$(nproc) mbstring
RUN usermod -u 1000 www-data

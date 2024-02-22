FROM wordpress:latest

RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

COPY ./xdebug.ini "${PHP_INI_DIR}/conf.d"
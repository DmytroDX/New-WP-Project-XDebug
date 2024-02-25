FROM wordpress:latest

RUN curl -fsSL https://deb.nodesource.com/setup_21.x | bash \
    && apt-get install -y nodejs

RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

COPY ./xdebug.ini "${PHP_INI_DIR}/conf.d"

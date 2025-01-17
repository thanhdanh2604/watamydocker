FROM php:7.3.15-fpm
RUN docker-php-ext-install pdo_mysql mysqli mbstring
RUN cd /usr/bin && curl -s http://getcomposer.org/installer | php && ln -s /usr/bin/composer.phar /usr/bin/composer
RUN apt-get update \
&& apt-get install -y \
git \
zip \
unzip \
vim
WORKDIR /src
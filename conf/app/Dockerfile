FROM php:5.6.31-apache

RUN apt-get update && apt-get install -y \
    vim \
    git \
    libfreetype6-dev \
    libjpeg62-turbo-dev \
    libmcrypt-dev \
    libpng12-dev \
    libmemcached-dev \
    zlib1g-dev \
    libpq-dev
RUN docker-php-ext-install -j$(nproc) iconv mcrypt pdo \
    pdo_mysql pgsql pdo_pgsql mysql mysqli json zip
RUN pecl install memcached-2.2.0
RUN docker-php-ext-enable memcached

COPY . /var/www/html/

RUN chmod -R 777 /var/www/html/app/cache/
RUN chmod -R 777 /var/www/html/app/logs/

RUN ln -sv /etc/apache2/mods-available/rewrite.load /etc/apache2/mods-enabled/rewrite.load
RUN cp -f /var/www/html/conf/app/qcharts.conf /etc/apache2/sites-available/000-default.conf


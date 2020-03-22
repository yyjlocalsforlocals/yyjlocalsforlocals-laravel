FROM php:fpm-alpine

ADD https://raw.githubusercontent.com/mlocati/docker-php-extension-installer/master/install-php-extensions /usr/local/bin/

RUN chmod uga+x /usr/local/bin/install-php-extensions && sync && \
    install-php-extensions gd xdebug bcmath mcrypt pdo_mysql mysqli redis zip

CMD ["php-fpm"]

EXPOSE 9000

ARG PHP_VERSION=8.5
ARG PHP_DIGEST
FROM serversideup/php:${PHP_VERSION}-cli${PHP_DIGEST}

USER root
RUN install-php-extensions bcmath exif gd imagick intl mysqli
USER www-data

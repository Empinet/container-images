ARG PHP_VERSION=8.5
ARG PHP_DIGEST
FROM serversideup/php:${PHP_VERSION}-frankenphp-trixie${PHP_DIGEST}

USER root
RUN install-php-extensions bcmath exif gd intl
# Retain the mbedTLS libraries provided by earlier upstream images.
RUN apt-get update && \
    apt-get install -y --no-install-recommends libmbedcrypto16 libmbedtls21 libmbedx509-7 && \
    rm -rf /var/lib/apt/lists/*
USER www-data

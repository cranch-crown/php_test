FROM php:7.3-fpm-alpine

ARG TZ

COPY php.ini /usr/local/etc/php

RUN apk --update add --no-cache tzdata && \
    cp /usr/share/zoneinfo/${TZ} /etc/localtime && \
    apk del tzdata
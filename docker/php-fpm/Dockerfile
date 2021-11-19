FROM php:8-alpine

WORKDIR /var/www
COPY ./task.txt ./

RUN echo "<?php phpinfo(INFO_GENERAL); ?>" > ./phpinfo.php

EXPOSE 8080

ENTRYPOINT ["php", "-S", "0.0.0.0:8080", "-t", "/var/www"]

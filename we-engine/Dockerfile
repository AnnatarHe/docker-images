FROM php:5.6
MAINTAINER AnnatarHe <iamhele1994@gmail.com>

RUN docker-php-ext-install pdo pdo_mysql
RUN apt-get update
RUN apt-get install -y libpng-dev libjpeg-dev
RUN docker-php-ext-install pdo pdo_mysql gd
RUN docker-php-ext-enable gd

WORKDIR /server

CMD ["/bin/bash"]

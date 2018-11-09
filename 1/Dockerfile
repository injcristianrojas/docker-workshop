# Build using docker build -t workshop1 .

FROM ubuntu:bionic

RUN apt-get update
RUN apt-get -y install nginx php-fpm
COPY default /etc/nginx/sites-available/default

EXPOSE 80

CMD "/bin/bash"
# run using docker run -p 80:80 -v {$PWD}/php:/var/www/html/php -i -t workshop1 /bin/bash
# service php7.2-fpm restart (status)
# service nginx restart

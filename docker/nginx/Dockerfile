FROM nginx:latest

COPY ssl/localhost.conf /etc/nginx/ssl/localhost.conf

RUN openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/nginx/ssl/localhost.key -out /etc/nginx/ssl/localhost.crt -config /etc/nginx/ssl/localhost.conf

WORKDIR /var/www/ib-proekt.com
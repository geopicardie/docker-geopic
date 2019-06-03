FROM debian:stretch-backports

RUN apt-get update && apt-get upgrade -y && apt-get install nginx -y
RUN apt-get install -y certbot python-certbot-nginx -t stretch-backports

CMD nginx -g 'daemon off ;';
ADD nginx.conf /etc/nginx/sites-enabled/default
EXPOSE 80

FROM alpine
MAINTAINER Michael Venezia <mike@cc.com>

EXPOSE 80 443

RUN apk update && apk add apache2 && apk add apache2-proxy

ADD website.conf /etc/apache2/conf.d/website.conf

ADD website /website

CMD apachectl -D FOREGROUND
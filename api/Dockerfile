FROM node:16-buster

RUN TZ=Asia/Tokyo

RUN mkdir -p /var/www/

ADD ./package.json /var/www/
#ADD ./package-lock.json /var/www/

WORKDIR /var/www

CMD npm ci --verbose && npm run serve:develop
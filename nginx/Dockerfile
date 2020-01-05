FROM nginx:alpine

RUN rm /etc/nginx/conf.d/default.conf

RUN apk --update add --no-cache\
        bash \
        sudo \
        nano \
        vim \
        curl

# clear cache
RUN rm -Rf /var/cache/apk/*

# nginx settings
RUN curl -o /etc/nginx/conf.d/default.conf https://raw.githubusercontent.com/JorgeEmanoel/docker/master/nginx/nginx.conf

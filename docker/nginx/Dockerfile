FROM alpine:3.6

RUN apk update && \
    apk add --no-cache nginx

ADD ./nuxt.conf /etc/nginx/conf.d/nuxt.conf
ADD ./rails.conf /etc/nginx/conf.d/rails.conf

RUN rm -rf /etc/nginx/conf.d/default.conf

EXPOSE 80
EXPOSE 8000


RUN mkdir -p /run/nginx

CMD nginx -g "daemon off;"

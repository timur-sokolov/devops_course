FROM alpine:latest

WORKDIR /web_app

RUN apk update && \
    apk add nginx

COPY ../configs/nginx/index.html /var/www/html/index.html

COPY ../configs/nginx/default.conf /etc/nginx/http.d/

CMD ["nginx", "-g", "daemon off;"]
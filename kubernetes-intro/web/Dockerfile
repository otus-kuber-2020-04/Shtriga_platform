FROM nginx:1.18.0-alpine

RUN deluser nginx && \
    adduser -s /sbin/nologin -h /var/cache/nginx -D -u 1001 -g nginx nginx && \
    touch /var/run/nginx.pid && chown nginx:nginx /var/run/nginx.pid

USER nginx

EXPOSE 8000

COPY infra/nginx/default.conf /etc/nginx/conf.d/default.conf

COPY app /app


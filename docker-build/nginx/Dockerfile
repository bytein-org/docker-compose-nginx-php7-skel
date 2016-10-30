FROM nginx:stable

COPY nginx.conf /etc/nginx/
COPY conf.d /etc/nginx/conf.d/

RUN usermod -u 1000 www-data

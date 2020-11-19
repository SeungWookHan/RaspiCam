FROM nginxinc/nginx-unprivileged:1-alpine

COPY ./default.conf /etc/ngingx/conf.d/default.conf
COPY ./uwsgi_params /etc/ngingx/uwsgi_params

USER root

RUN mkdir -p /vol/static
RUN chmod 755 /vol/static

USER nginx
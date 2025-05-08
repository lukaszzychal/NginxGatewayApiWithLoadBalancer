FROM nginx:1.23.1-alpine

RUN rm /etc/nginx/conf.d/default.conf

COPY ./nginx.conf /etc/nginx/nginx.conf
#COPY ./nginx.conf /etc/nginx/conf.d/default.conf

COPY ./api_gateway.conf /etc/nginx/api_gateway.conf
COPY ./api_backends.conf /etc/nginx/api_backends.conf
COPY ./api_json_errors.conf /etc/nginx/api_json_errors.conf
COPY ./api_keys.conf /etc/nginx/api_keys.conf
COPY ./api_conf.d /etc/nginx/api_conf.d/


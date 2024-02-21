FROM nginx:latest

COPY nginx.template.conf /nginx.template.conf

ENV AUTH_SERVICE_NEST_ADDRESS 10.5.0.3
ENV POSTGRES_DB_ADDRESS 10.5.0.2
ENV POSTGRES_ADMIN_PANEL_ADDRESS 10.5.0.4

CMD ["/bin/sh" , "-c" , "envsubst '${AUTH_SERVICE_NEST_ADDRESS},${POSTGRES_DB_ADDRESS},${POSTGRES_ADMIN_PANEL_ADDRESS}' < /nginx.template.conf > /etc/nginx/nginx.conf && exec nginx -g 'daemon off;'"]

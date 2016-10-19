FROM nginx:1.11.5

COPY nginx.template /etc/nginx/nginx.template

# Hacemos sustitución de variables de entorno en el archivo de configuración
CMD /bin/bash -c "envsubst < /etc/nginx/nginx.template > /etc/nginx/nginx.conf && nginx -g 'daemon off;'"

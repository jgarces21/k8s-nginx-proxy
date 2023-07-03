FROM nginx:1.19.3-alpine
COPY nginx.conf /etc/nginx/templates/default.conf.template
COPY src /usr/share/nginx/html
RUN chown -R nginx:nginx /etc/nginx && chown -R nginx:nginx /var/cache/nginx && chown -R nginx:nginx /usr/share/nginx/ && chown -R nginx:nginx /var/log/nginx/ && chmod -R ugo+rw /var/run/
USER nginx

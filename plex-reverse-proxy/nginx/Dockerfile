FROM nginx:alpine

RUN mkdir -p /etc/nginx/includes
COPY conf/nginx.conf /etc/nginx/nginx.conf
COPY conf/plex-proxy.conf /etc/nginx/includes/plex-proxy.conf

# HEALTHCHECK --interval=10s --timeout=3s --start-period=30s --retries=3 \
#     CMD curl --fail http://localhost/healthz || exit 1  
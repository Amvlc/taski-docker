FROM nginx:1.22.1

# Create SSL directory
RUN mkdir -p /etc/nginx/ssl

# Copy SSL certificates
COPY ssl/fullchain.pem /etc/nginx/ssl/
COPY ssl/privkey.pem /etc/nginx/ssl/

# Copy nginx configuration
COPY conf.d/default.conf /etc/nginx/conf.d/default.conf

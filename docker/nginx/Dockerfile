FROM nginx:latest

# Copy nginx configuration
COPY docker/nginx/nginx.conf /etc/nginx/nginx.conf

# Set working directory
WORKDIR /usr/share/nginx/html

# Copy all web files
COPY front/ .

# Set permissions
RUN chown -R nginx:nginx /usr/share/nginx/html && \
    chmod -R 755 /usr/share/nginx/html

EXPOSE 80
# Use the official Nginx image
FROM nginx:latest

# Copy front-end files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom Nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

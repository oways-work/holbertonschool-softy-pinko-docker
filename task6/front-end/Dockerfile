# Use the official Nginx image as the base
FROM nginx:latest

# Copy the cloned front-end repository files to the location Nginx expects
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy your custom Nginx configuration file, replacing the default Nginx config
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
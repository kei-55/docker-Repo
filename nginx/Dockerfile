FROM nginx:latest

# Copy custom configuration file to the container
COPY nginx.conf /etc/nginx/nginx.conf

# Copy static files to the container
COPY ./web /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start nginx server
CMD ["nginx", "-g", "daemon off;"]
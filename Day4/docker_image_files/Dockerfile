#  the base image
FROM nginx:latest

# Copy the configuration file
COPY ./nginx.conf /etc/nginx/nginx.conf

# Specify the command to run when starting the container
CMD ["nginx", "-g", "daemon off;"]

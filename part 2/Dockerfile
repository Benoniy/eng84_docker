# Define the base image 
# You can do this using the keyword FROM
FROM nginx
LABEL MAINTAINER = branson@spartaglobal.com

# COPY something into the base image
COPY index.html /usr/share/nginx/html/index.html

# Expose port 80
EXPOSE 80

# Executes a command
CMD ["nginx", "-g", "daemon off;"]
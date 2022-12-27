FROM nginx

#Default configuration for Proxy Service 
COPY default.conf /etc/nginx/conf.d/default.conf

#HTML Error Responses
COPY backend-not-found.html /var/www/html/backend-not-found.html

#Proxy configurations
COPY ./includes/ /etc/nginx/includes/

#SSL Certificates
COPY ./ssl/ /etc/ssl/certs/nginx/

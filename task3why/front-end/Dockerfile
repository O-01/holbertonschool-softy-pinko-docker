# container base image as latest version of nginx
FROM nginx:latest

# copy input front-end files to specified output location within container
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# copy input nginx conf to specified output location within container
COPY ./softy-pinko-front-end.conf  /etc/nginx/conf.d/default.conf

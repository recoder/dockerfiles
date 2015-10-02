FROM rails:latest
MAINTAINER Andrew Kondrashov <recoder@gmail.com>

RUN apt-get update

# Install Nginx.
RUN apt-get install -qq -y nginx
RUN echo "\ndaemon off;" >> /etc/nginx/nginx.conf
RUN chown -R www-data:www-data /var/lib/nginx

# Install foreman
RUN gem install foreman

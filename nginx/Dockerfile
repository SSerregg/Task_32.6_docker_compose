FROM ubuntu:latest
RUN apt-get update
RUN apt-get install -y nginx
COPY ./hosts/application.conf /etc/nginx/sites-enabled/application.conf
WORKDIR /data
VOLUME /data
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
FROM ubuntu:latest
LABEL microservicehost="Vr-website"
RUN apt update
RUN apt install nginx -y &&\ apt install vim -y
RUN rm -rf /var/www/html/index.html
WORKDIR /var/www/html/
COPY . .
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
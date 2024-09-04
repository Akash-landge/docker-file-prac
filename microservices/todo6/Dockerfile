FROM ubuntu
LABEL akash="07"
RUN apt update &&\
    apt install nginx -y &&\
    apt install vim -y
RUN rm -rf /var/www/html/*
WORKDIR /var/www/html/
COPY . .
EXPOSE 80
#CMD ["apache2ct" , "-DFOREGROUND"]
CMD ["nginx", "-g", "daemon off;"]
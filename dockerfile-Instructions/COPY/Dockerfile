FROM almalinux:9
RUN yum install nginx -y 
RUN rm /usr/share/nginx/html/index.html

COPY index.html /usr/share/nginx/html/ 
CMD ["nginx", "-g", "daemon off;"]
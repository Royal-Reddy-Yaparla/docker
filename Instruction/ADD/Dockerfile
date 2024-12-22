FROM almalinux:9
RUN yum install nginx -y 

RUN rm /usr/share/nginx/html/index.html
ADD index.html /usr/share/nginx/html/
 
ADD https://filesamples.com/samples/document/txt/sample3.txt /tmp/
ADD sample-1.tar /tmp/

CMD ["nginx", "-g", "daemon off;"]
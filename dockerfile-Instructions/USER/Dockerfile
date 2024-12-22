FROM almalinux:9 
RUN adduser bob
USER bob
RUN yum install nginx -y 
CMD ["nginx","-g","daemon off;"]
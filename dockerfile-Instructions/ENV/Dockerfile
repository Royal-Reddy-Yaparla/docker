FROM almalinux:9 
RUN yum install nginx -y 
ENV PROJECT="fusion" \
    ENVIRONMENT="dev" \
    TEAM="testing"
CMD [ "nginx", "-g", "deamon off;" ]
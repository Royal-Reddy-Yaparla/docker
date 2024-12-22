FROM almalinux:9 
LABEL PROJECT="fusion" \
      TEAM="devops" \
      CREATED="EMP-1234"
      
RUN yum install nginx -y 
ENV PROJECT="fusion" \
    ENVIRONMENT="dev" \
    TEAM="testing"
CMD [ "nginx", "-g", "deamon off;" ]
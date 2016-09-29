FROM centos:latest
MAINTAINER Walt Byte <walt@gbyte.co>

RUN yum -y update \
    && yum -y install epel-release \
    && yum -y install nginx \
    && yum clean all

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]

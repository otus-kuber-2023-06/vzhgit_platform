FROM centos:centos7
RUN mkdir /app/
RUN yum -y install epel-release
RUN yum -y install nginx
RUN usermod -u 1001 nginx && groupmod -g 1001 nginx
ADD app.conf /etc/nginx/conf.d/app.conf
EXPOSE 8000
CMD ["nginx", "-g", "daemon off;"]

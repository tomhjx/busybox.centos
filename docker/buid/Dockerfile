# Dockerfile - CentOS 7
FROM centos:7

LABEL maintainer="Tom <tom_hejiaxi@163.com>"

RUN yum install -y \
        gcc \
        gcc-c++ \
        gd-devel \
        gettext \
        GeoIP-devel \
        libxslt-devel \
        make \
        perl \
        perl-ExtUtils-Embed \
        readline-devel \
        unzip \
        zlib-devel \
        patch \
        httpd-tools \
        nfs-utils \ 
        inotify-tools

COPY start.sh /start.sh

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && chmod +x /start.sh

CMD ["/start.sh"]
FROM centos:7
MAINTAINER info@signalsciences.com
RUN set -ex \
    && yum install -y rpm-build ruby rubygems \
    && yum install -y gcc ruby-devel make \
    && gem install --no-ri --no-rdoc fpm \
    && yum remove -y gcc ruby-devel make \
    && yum clean all

ENTRYPOINT [ "/usr/local/bin/fpm" ]

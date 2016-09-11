FROM alpine:3.4
MAINTAINER info@signalsciences.com
# must use GNU tar, not busybox
RUN set -ex \
    && apk add --update gcc libc-dev ruby ruby-dev libffi libffi-dev make tar \
    && gem install --no-ri --no-rdoc fpm \
    && apk del gcc libc-dev ruby-dev libffi-dev make
ENTRYPOINT [ "/usr/bin/fpm" ]

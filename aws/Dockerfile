FROM alpine:3.3
MAINTAINER info@signalsciences.com
RUN set -ex \
    && apk add --update python python-dev py-pip gcc libc-dev \
    && pip install aws \
    && apk del python-dev gcc libc-dev
ENTRYPOINT [ "/usr/bin/aws" ]

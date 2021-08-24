FROM ttbb/base

LABEL maintainer="shoothzj@gmail.com"

ENV HEARTBEAT_HOME /opt/sh/heartbeat

ARG download=7.14.0-linux-x86_64

RUN wget https://artifacts.elastic.co/downloads/beats/heartbeat/heartbeat-$download.tar.gz && \
mkdir /opt/sh/heartbeat && \
tar -xf heartbeat-$download.tar.gz -C /opt/sh/heartbeat --strip-components 1 && \
rm -rf /opt/sh/heartbeat-$download.tar.gz

WORKDIR /opt/sh/heartbeat
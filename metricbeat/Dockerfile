FROM ttbb/base

LABEL maintainer="shoothzj@gmail.com"

ARG download=7.14.0-linux-x86_64

RUN wget https://artifacts.elastic.co/downloads/beats/metricbeat/metricbeat-$download.tar.gz && \
mkdir /opt/sh/metricbeat && \
tar -xf metricbeat-$download.tar.gz -C /opt/sh/metricbeat --strip-components 1 && \
rm -rf /opt/sh/metricbeat-$download.tar.gz

WORKDIR /opt/sh/metricbeat
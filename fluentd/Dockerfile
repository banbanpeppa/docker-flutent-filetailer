FROM fluent/fluentd:v1.12.0-debian-1.0

USER root
WORKDIR /home/fluent

RUN gem install fluent-plugin-record-reformer \
    && gem install fluent-plugin-forest 
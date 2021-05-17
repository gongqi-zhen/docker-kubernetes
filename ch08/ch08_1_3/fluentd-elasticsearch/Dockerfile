# fluentd/Dockerfile
#FROM fluent/fluentd:v0.12-debian
# https://qiita.com/myoshimi/items/ad14339f4be82d24b5f5
# version change
FROM fluent/fluentd:v1.3.2
RUN ["gem", "install", "fluent-plugin-elasticsearch", "--no-rdoc", "--no-ri", "--version", "1.9.2"]
COPY fluent.conf /fluentd/etc/fluent.conf


ARG TAG=centos7
ARG PLATFORM=linux/amd64
FROM --platform $PLATFORM quay.io/centos/centos:$TAG
MAINTAINER TiMoR <https://timor.site>

# upgrade packages
RUN yum upgrade -y && \
    yum clean all && \
    rm -rf /tmp/* && \
    rm -rf /var/cache/yum && \
    find /var/log -type f -name '*.log' -delete

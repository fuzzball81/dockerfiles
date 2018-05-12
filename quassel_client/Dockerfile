# Dockerfile for quassel client on fedora
FROM fedora:latest

MAINTAINER Jason Joyce

RUN dnf -y install quassel-client && \
    dnf -y clean all

ADD ./quassel-run.sh /usr/local/sbin/quassel-run.sh

ENTRYPOINT ["/usr/local/sbin/quassel-run.sh"]


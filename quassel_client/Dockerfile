# Dockerfile for quassel client on fedora
FROM fedora:27

MAINTAINER Jason Joyce

RUN dnf -y install quassel-client && \
    dnf -y clean all

ADD ./quassel-run.sh /usr/local/sbin/quassel-run.sh

ENTRYPOINT ["/usr/local/sbin/quassel-run.sh"]


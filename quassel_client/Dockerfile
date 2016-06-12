# Dockerfile for quassel client on fedora
FROM fedora:latest

MAINTAINER Jason Joyce

RUN dnf -y upgrade && \
    dnf -y install quassel-client && \
    dnf -y clean all

ADD ./quassel-run.sh /usr/local/sbin/quassel-run.sh

CMD ["/usr/local/sbin/quassel-run.sh"]


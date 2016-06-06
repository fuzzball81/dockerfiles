# Dockerfile for quassel client on fedora
FROM fedora:latest

MAINTAINER Jason Joyce

RUN dnf -y upgrade
RUN dnf -y install quassel-client
ADD ./quassel-run.sh /usr/local/sbin/quassel-run.sh

CMD ["/usr/local/sbin/quassel-run.sh"]


FROM ubuntu:14.04
MAINTAINER Dean Kayton <deankayton@gmail.com>

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y software-properties-common && \
    apt-add-repository ppa:ubuntu-mate-dev/ppa && \
    apt-add-repository ppa:ubuntu-mate-dev/trusty-mate && \
    apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y ubuntu-mate-core && \
    apt-get install -y ubuntu-mate-desktop && \
    apt-get install -y xrdp
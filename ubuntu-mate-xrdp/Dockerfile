FROM ubuntu:14.04
MAINTAINER "Dean Kayton <deankayton@gmail.com>"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    software-properties-common
RUN apt-add-repository \
    ppa:ubuntu-mate-dev/ppa \
    ppa:ubuntu-mate-dev/trusty-mate
RUN apt-get update && apt-get upgrade -y && apt-get install -y \
    ubuntu-mate-core \
    ubuntu-mate-desktop \
    xrdp
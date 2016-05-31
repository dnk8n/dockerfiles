FROM ubuntu:trusty
MAINTAINER Dean Kayton <deankayton@gmail.com>
ENV DEBIAN_FRONTEND noninteractive
RUN dpkg --add-architecture i386
RUN apt-get update && apt-get -y install \
    firefox:i386 \
    fonts-takao \
    icedtea-7-plugin:i386 \
    libpangox-1.0-0:i386 \
    libpangoxft-1.0-0:i386 \
    libxft2:i386 \
    libxmu6:i386 \
    libxv1:i386 \
    openjdk-7-jre:i386
ARG webex_passw
RUN adduser --quiet --disabled-password --gecos "" webex && echo "webex:${webex_passw}" | chpasswd
USER webex
WORKDIR /home/webex/
ENTRYPOINT ["/bin/bash"]
CMD ["/usr/bin/firefox", "go.webex.com"]
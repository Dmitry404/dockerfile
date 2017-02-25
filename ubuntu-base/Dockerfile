# Base Ubuntu image for my needs
FROM ubuntu:16.04
MAINTAINER dmitry404@gmail.com

RUN apt-get update && apt-get install -y --no-install-recommends \
    bzip2 \
    unzip \
    xz-utils \
    wget \
    vim \
    bash-completion \
  && rm -rf /var/lib/apt/lists/*

CMD ["/bin/bash"]

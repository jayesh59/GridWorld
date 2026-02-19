FROM ubuntu:24.04
ARG DEBIAN_FRONTEND=noninteractive
ENV QT_X11_NO_MITSHM=1

RUN apt update && apt install -q -y --no-install-recommends software-properties-common
RUN add-apt-repository -y ppa:deadsnakes/ppa && \
    apt update && apt install -q -y --no-install-recommends \
        python3.10 \
        python3.10-dev

RUN apt update && apt install -q -y --no-install-recommends \
        git \
        neovim \
        vim  \
        tmux  \
        wget  \
        curl  \
        openssh-client  \
        software-properties-common \
        btop \
        net-tools \
        python3-pip \
        libreoffice-writer \
        libreoffice-calc \
        iputils-ping \
        tree \
        lsb-release \
        mesa-utils

RUN apt-get update && apt-get install --upgrade -q -y --no-install-recommends xauth xorg openbox

WORKDIR /root/lab_git/
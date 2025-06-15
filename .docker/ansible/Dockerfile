FROM ubuntu:24.04

RUN apt update && \
    apt upgrade -y && \
    apt install -y ansible openssh-client && \
    echo 'root:root' | chpasswd

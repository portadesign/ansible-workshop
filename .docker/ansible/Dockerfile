FROM ubuntu:24.04

RUN apt update && \
    apt upgrade -y && \
    apt install -y ansible curl openssh-client sshpass && \
    echo 'root:root' | chpasswd

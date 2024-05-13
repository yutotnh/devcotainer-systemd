FROM centos:centos7

# Add non-root user
RUN useradd -s /bin/bash -m vscode \
# Add sudo support for the non-root user
    && yum install -y sudo \
    && echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

ENTRYPOINT ["/sbin/init"]

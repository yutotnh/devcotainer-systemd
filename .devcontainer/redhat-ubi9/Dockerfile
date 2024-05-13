FROM redhat/ubi9

# Add non-root user
RUN useradd -s /bin/bash -m vscode \
# Add sudo support for the non-root user
    && dnf install -y sudo \
    && echo "vscode ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

ENTRYPOINT ["/sbin/init"]

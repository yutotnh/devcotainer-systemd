FROM mcr.microsoft.com/devcontainers/base:jammy

RUN \
    # Install dependencies
    apt-get update \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
    systemd \
    # Link systemd to /sbin/init
    && ln -sf /lib/systemd/systemd /sbin/init \
    # Remove dummy systemd
    && rm -f /usr/local/bin/systemctl \
    # Clean up
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/sbin/init"]

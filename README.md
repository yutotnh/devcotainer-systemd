# systemd On Dev container

## Description

This is a simple example of how to use systemd on a dev container.

## How to use

1. Clone this repository

2. Open the repository in VS Code

3. Install the Remote - Containers extension

4. Reopen the repository in a container

## Distribution

| Distribution | Version | Dockerfile                                            | Note                                                                |
| ------------ | ------- | ----------------------------------------------------- | ------------------------------------------------------------------- |
| Ubuntu       | 22.04   | [Dockerfile](./.devcontainer/ubuntu-jammy/Dockerfile) |                                                                     |
| Red Hat      | 9       | [Dockerfile](./.devcontainer/redhat-ubi9/Dockerfile)  |                                                                     |
| CentOS       | 7       | [Dockerfile](./.devcontainer/centos7/Dockerfile)      | It works only in environments where cgroup is v1, such as CentOS 7. |

## License

MIT License

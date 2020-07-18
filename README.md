# docker_ce

An Ansible role to install docker and docker compose

## Variables

docker_ce_package:
  - Defaulted to 'docker-ce'

docker_ce_install_compose:
  - Install docker compose True/ False

docker_ce_compose_version:
  - Composer version to be installed

docker_ce_users:
  - List of users added to docker group.

## Examples

Install docker community edition

```
- role: docker_ce

- role: docker_ce
  docker_ce_users:
    - '{{ docker_users }}'

```

# Platform Support
Role supports installation of docker & docker-compose packages on
  - Debian
  - Redhat
  - AmazonLinux2

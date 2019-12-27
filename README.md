# docker

Install docker, docker-compose.

## Requirements

None.

## Role Variables

- DOCKER_USER

  Default: docker

  User to create which docker containers run as.

- DOCKER_CE_REPO

  Default: https://mirrors.aliyun.com/docker-ce/linux/centos/docker-ce.repo

  Docker CE repository url.

- DOCKER_INSTALL_COMPOSE

  Default: true

  Control whether install docker-compose.

- DOCKER_COMPOSE_VERSION

  Default: 1.25.0

  The version of docker-compose to install.

- DOCKER_COMPOSE_PATH

  Default: /usr/loca/bin/docker-compose

  The path of docker-compose to install.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers

  roles:
    - role: aeternuss.docker
      vars:
        docker_compose_version: "1.25.0"
```

## License

GPL-3.0

## Author Information

Author: aeternus

Email: aeternus@aliyun.com

Site: [Aeternus](https://aeternus.cc)

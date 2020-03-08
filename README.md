# Ansible role for Docker

This is a simple role for Debian that will Install docker-ce from the official APT repo + docker-compose + a cron to cleanup old images.

## Installation

Add this to your `requirements.yml`:

```yml
- src: https://github.com/angristan/ansible-docker
```

## Sample playbook

```yaml
---

- hosts: myhost
  roles:
    - {role: docker, tags: docker}
```

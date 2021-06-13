# Ansible role for Docker

This is a simple role for Debian that will Install docker-ce from the official APT repo + docker-compose + a cron to cleanup old images.

## Usage

Add this to `requirements.yml`:

```yml
- src: https://github.com/angristan/ansible-base
  name: angristan.base
  version: vX.X.X
```

### Sample playbook

```yaml
---
- hosts: myhost
  roles:
    - { role: docker, tags: docker }
```

## Author Information

See my other Ansible roles at [angristan/ansible-roles](https://github.com/angristan/ansible-roles).

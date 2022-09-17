[![CI](https://github.com/de-it-krachten/ansible-role-docker_compose/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-docker_compose/actions?query=workflow%3ACI)


# ansible-role-docker_compose

Installs docker-compose

## Platforms

Supported platforms

- Red Hat Enterprise Linux 7<sup>1</sup>
- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- CentOS 7
- RockyLinux 8
- RockyLinux 9
- OracleLinux 8
- AlmaLinux 8
- AlmaLinux 9
- Debian 10 (Buster)
- Debian 11 (Bullseye)
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS
- Fedora 35
- Fedora 36

Note:
<sup>1</sup> : no automated testing is performed on these platforms

## Role Variables
### defaults/main.yml
<pre><code>
# type of installation (binary/pip/both)
docker_compose_type: binary

# API endpoint to get latest version 
docker_compose_api: https://api.github.com/repos/docker/compose

# Download location for binary
docker_compose_repo: https://github.com/docker/compose

# Should the software be downloaded
docker_compose_download: true

# Version to install
docker_compose_version: latest

# Platform/architecture, as it makes part of the binary to download
docker_compose_platform: "{{ ansible_system | lower }}-{{ ansible_architecture }}"

# Target location/ownership/permissions for the binary
docker_compose_path: /usr/local/bin/docker-compose
docker_compose_owner: root
docker_compose_group: root
docker_compose_mode: '0755'
</pre></code>



## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'docker_compose'
  hosts: all
  become: "{{ molecule['converge']['become'] | default('yes') }}"
  tasks:
    - name: Include role 'docker_compose'
      include_role:
        name: docker_compose
</pre></code>

[![CI](https://github.com/de-it-krachten/ansible-role-docker_compose/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-docker_compose/actions?query=workflow%3ACI)


# ansible-role-docker_compose

Installs docker-compose



## Dependencies

#### Roles
None

#### Collections
- community.docker

## Platforms

Supported platforms

- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- RockyLinux 8
- RockyLinux 9
- OracleLinux 8
- OracleLinux 9
- AlmaLinux 8
- AlmaLinux 9
- SUSE Linux Enterprise 15<sup>1</sup>
- openSUSE Leap 15
- Debian 11 (Bullseye)
- Debian 12 (Bookworm)<sup>1</sup>
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS
- Ubuntu 24.04 LTS
- Fedora 40<sup>1</sup>
- Fedora 41<sup>1</sup>
- Alpine 3<sup>1</sup>

Note:
<sup>1</sup> : no automated testing is performed on these platforms

## Role Variables
### defaults/main.yml
<pre><code>
# -----------------------------------------------------------------------------
# Install
# -----------------------------------------------------------------------------

# type of installation (binary/pip/both)
docker_compose_type: pip

# Should docker-compose be installed into a venv
docker_compose_pipinvenv: true

# Set virtual environment location
docker_compose_venv_path: /usr/local/venv/docker-compose

# Python to use for docker-compose in venv
docker_compose_venv_python: /usr/bin/python3

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

# Default permissions for data directories
docker_compose_owner: root
docker_compose_group: root
docker_compose_mode: '0755'


# -----------------------------------------------------------------------------
# Template
# -----------------------------------------------------------------------------

# Path where docker-compose projects can be found
docker_compose_root: /export/docker

# Specifies project location
docker_compose_project_dir: "{{ docker_compose_root }}/{{ docker_compose_project_name }}"

# Should the latest image be pulled during project start/restart (always, missing)
docker_compose_pull: missing

# Should the latest image be build during project start/restart (always, missing)
docker_compose_build: never

# Force restart of the project (by default only when a change is found)
docker_compose_restart: false

# Execute template code as root
docker_compose_become: no
</pre></code>




## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'docker_compose'
  hosts: all
  become: 'yes'
  vars:
    python_package_install_optional: true
    docker_compose_type: pip
  roles:
    - deitkrachten.python
  tasks:
    - name: Include role 'docker_compose'
      ansible.builtin.include_role:
        name: docker_compose
</pre></code>

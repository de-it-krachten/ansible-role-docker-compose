[![CI](https://github.com/de-it-krachten/ansible-role-docker_compose/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-docker_compose/actions?query=workflow%3ACI)


# ansible-role-docker_compose

Installs docker-compose

Platforms
--------------

Supported platforms

- CentOS 7
- CentOS 8
- RockyLinux 8
- AlmaLinux 8
- Debian 10 (Buster)
- Debian 11 (Bullseye)
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS



Role Variables
--------------
<pre><code>

</pre></code>


Example Playbook
----------------

<pre><code>
- name: sample playbook for role 'docker_compose'
  hosts: all
  vars:
  tasks:
    - name: Include role 'docker_compose'
      include_role:
        name: docker_compose
</pre></code>

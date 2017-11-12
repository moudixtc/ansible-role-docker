moudixtc.docker
=========

Installs docker-ce, and/or docker-compose.

Requirements
------------

N/A

Role Variables
--------------

Refer to the [defaults](defaults/main.yml) and all the package manager and distribution specific variables in `/vars` directory.

Dependencies
------------

N/A

Example Playbook
----------------

Basic install with docker and docker-compose. Also add ubuntu user to docker's group:
```yamlex
- hosts: localhost
  tasks:
    - include_role:
        name: moudixtc.docker
      vars:
        docker_compose_install: yes
        docker_group_users:
          - ubuntu
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

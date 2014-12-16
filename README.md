Ansible DotDeb repository playbook
=====

This role installs and configures DotDeb on a server.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

```
dotdeb_repo_version: wheezy
dotdeb_extra_repo: True
dotdeb_extra_repo_version: wheezy-php56
```

Examples
========

```
# Roles
- name: log server
  hosts: logs
  user: root
  roles:
    - dotdeb
  vars_files:
    - "host_vars/dotdeb.yml"

```

Dependencies
------------

None

License
-------

GPL

Author Information
------------------

Pierre Mavro / deimosfr



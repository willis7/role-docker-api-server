Docker API Server
=========

This Ansible playbook modifies `daemon.json` in order to enable the API Server.

Role Variables
--------------

`defaults/main.yml` includes a config section which is used to populate `daemon.json`.

Example Playbook
----------------

``` yaml
- name: Enable Docker API
  hosts: swarm-first-manager
  become: true
  roles:
    - {role: docker-api-server}
```

Author Information
------------------

* Sion Williams (sion.williams@ext.ons.gov.uk)


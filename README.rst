=====================
ansible-role-grafyaml
=====================

Ansible role to setup and configure grafana using grafyaml

* License: Apache License, Version 2.0
* Documentation: https://docs.openstack.org/infra/grafyaml
* Source: https://git.openstack.org/cgit/openstack/ansible-role-grafyaml
* Bugs: https://bugs.launchpad.net/ansible-role-grafyaml

Description
-----------

Grafyaml takes simple descriptions of Grafana dashboards in YAML format,
and uses them to configure Grafana. This ansible role installs grafyaml,
then imports dashboards using it into an existing grafana install.

Requirements
------------

See `bindep.txt` for role dependencies.

Packages
~~~~~~~~

Package repository index files should be up to date before using this role, we
do not manage them.

Role Variables
--------------

Dependencies
------------

Example Playbook
----------------

.. code-block:: yaml

    - name: Install grafyaml
      hosts: grafana
      roles:
        - ansible-role-grafyaml

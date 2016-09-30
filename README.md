Ansible Role: TowerCLI
==========================

[![Build Status](https://travis-ci.org/Aplyca/ansible-role-towercli.svg?branch=master)](https://travis-ci.org/Aplyca/ansible-role-towercli)
[![Circle CI](https://circleci.com/gh/Aplyca/ansible-role-towercli.png?style=badge)](https://circleci.com/gh/Aplyca/ansible-role-towercli)

Ansible Role for standard creation of roles.

Requirements
------------

Use hash behavior for variables in ansible.cfg
See example: https://github.com/Aplyca/ansible-role-towercli/blob/master/tests/ansible.cfg
See official docs: http://docs.ansible.com/intro_configuration.html#hash-behaviour

Installation
------------

Using ansible galaxy:
```bash
ansible-galaxy install Aplyca.TowerCLI
```
You can add this role as a dependency for other roles, add the role to the meta/main.yml file of your own role:
```yaml
dependencies:
  - { role: Aplyca.TowerCLI }
```

Role Variables
--------------

See default variables: https://github.com/Aplyca/ansible-role-towercli/blob/master/defaults/main.yml

Cretae a new role using this as boilerplate
-------------------------------------------

```bash
find ./ -type f -exec sed -i '' -e 's/towercli/newrole/g' {} \;
find ./ -type f -exec sed -i '' -e 's/Tower CLI/New Role/g' {} \;
find ./ -type f -exec sed -i '' -e 's/TowerCLI/NewRole/g' {} \;
```


Dependencies
------------

None.

Testing
-------
Using Vagrant:

```bash
tests/vagrant.sh
```
Using Docker:

```bash
tests/docker.sh
```

License
-------

MIT / BSD

Author Information
------------------

Mauricio Sánchez from Aplyca SAS (http://www.aplyca.com)

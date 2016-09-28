git-ubuntu
===========

[![Build Status](https://travis-ci.org/suzuki-shunsuke/ansible-git-ubuntu.svg?branch=master)](https://travis-ci.org/suzuki-shunsuke/ansible-git-ubuntu)

Install git on Ubuntu.

https://galaxy.ansible.com/suzuki-shunsuke/git-ubuntu/

Requirements
------------

Nothing.

Role Variables
--------------

* git_use_ppa: Whether use ppa to install git or not. The default value is "no".
* git_upgrade: Whether upgrade git if git has already installed. The default value is "no".
* git_nonroot: Whether the remote_user is root or not. This variable is set automatically, and is used to execute tasks with the become option.

Dependencies
------------

Nothing.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
  - role: suzuki-shunsuke.git-ubuntu
    git_use_ppa: yes
    git_upgrade: no
```

License
-------

MIT

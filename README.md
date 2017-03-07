ansible sshd-config
===================
[![Build Status](https://travis-ci.org/ypsman/ansible-sshd-config.svg?branch=master)](https://travis-ci.org/ypsman/ansible-sshd-config)

This Role configures sshd configures.

Config SSH daemon, root Login and Password Auth

Default option is to
      PermitRootLogin yes           # do not allow Root to login via ssh
      PasswordAuthentication no     # Only login with SSH-Key

Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.sshd-config
          sshd_PermitRootLogin: yes           # optional  
          sshd_PasswordAuthentication: no     # optional

ansible sshd-config
===================
[![Build Status](https://travis-ci.org/ypsman/ansible-sshd-config.svg?branch=master)](https://travis-ci.org/ypsman/ansible-sshd-config)

This Role Changes sshd config.

Variables to configure are:

    PermitRootLogin
    PasswordAuthentication
    ListenAddress

It also Validates the Conifg before<br>
restarting the deamon.


Example Playbook
----------------

    - hosts: all
      roles:
        - role: ypsman.sshd-config
          sshd_PermitRootLogin: 'no'
          sshd_PasswordAuthentication: 'no'
          sshd_ListenAddress: '0.0.0.0'

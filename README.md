Ansible Role: Windows SSH
=========

An Ansible role to install and configure OpenSSH on a Windows host.

Requirements
------------

None.

Role Variables
--------------

```yml
windows_ssh_download_path: '{{ ansible_env.TEMP | default(ansible_env.TMP) }}\OpenSSH'
windows_ssh_install_path: 'C:\Program Files\OpenSSH'
windows_ssh_pubkeys_enabled: true
windows_ssh_passwords_enabled: true
windows_ssh_public_keys: 
  - ssh public key
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yml
- hosts: servers
  roles:
    - role: xbufu.windows_ssh
```

License
-------

MIT / BSD

Author Information
------------------

Created by xbufu.

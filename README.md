Ansible Role: OpenShift Provider `KVM`
=========

This role help install/config KVM on Fedora.

*Details*
- Install KVM
- Add a new virtual network to KVM
- Add a new storage pool to KVM

Requirements
------------
None

Role Variables
--------------

| Name                  | Default value           | Requird | Description                              |
| --------------------- | ----------------------- | ------- | ---------------------------------------- |
| kvm_log_dir           | /tmp/kvm                | no      | Where role related config/log file store |
| kvm_storage_pool_name | Public                  | no      | Where Storage Pool Name                  |
| kvm_storage_pool_dir  | /var/lib/libvirt/images | no      | Where Storage Pool directory             |
| kvm_install_host      | localhost               | no      | Where KVM will install or installed      |


Dependencies
------------

None



Example Playbook
----------------
~~~
- name: Example Playbook
  hosts: localhost
  tasks:
    - include_role:
        name: ansible-role-kvm-provider-okd
~~~

License
-------

BSD/MIT

Author Information
------------------

This role was created in 2018 by [Jooho Lee](http://github.com/jooho).

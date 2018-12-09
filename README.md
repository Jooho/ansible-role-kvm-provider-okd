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

| Name                      | Default value                         |        Requird       | Description                                                                 |
|---------------------------|---------------------------------------|----------------------|-----------------------------------------------------------------------------|
| kvm_log_dir               | /tmp/kvm                              |         no           | Where role related config/log file store                                    |
| kvm_vm_pool_dir           | /var/lib/virt/images                  |         no           | Where VM images store                                                       |
| kvm_install_host          | localhost                             |         no           | Where KVM will install or installed                                         |


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
        name: Jooho.kvm_provider_okd
~~~

License
-------

BSD/MIT

Author Information
------------------

This role was created in 2018 by [Jooho Lee](http://github.com/jooho).

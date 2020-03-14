Role Name
=========

kvm 

Requirements
------------
* pipenv
* yimeng.proxmox galaxy role
* ansible

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- hosts: proxmox
  remote_user: root
  roles:

  # create kvm with auto get vm_id
  - { role: yimeng.proxmox,state: "present"}

  # delete kvm with given vm_id 112
  - { role: yimeng.proxmox,vm_id: "112",state: "absent"}

hosts:
[proxmox]
127.0.0.1
[proxmox:vars]
api_username="root@pam"
api_password=""
api_host="127.0.0.1"

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

UFW Role
=========

[![Build Status](https://travis-ci.org/mbreisch/ufw-role.svg?branch=master)](https://travis-ci.org/mbreisch/ufw-role)

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Defaults:
* ufw_allow_ipv6: "no"
* ufw_port_rules: []
* ufw_app_rules: []
* ufw_allow_ipv6: "no"
* ufw_default_input_policy: "DROP"
* ufw_default_ouput_policy: "ACCEPT"
* ufw_default_forward_policy: "DROP"
* ufw_default_application_policy: "SKIP"
* ufw_logging: "on"
* ufw_state: enabled
* 
```
ufw_policies:
    - { direction: 'incoming', policy: 'reject' }
    - { direction: 'outgoing', policy: 'allow' }
    - { direction: 'routed', policy: 'deny'}
```

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

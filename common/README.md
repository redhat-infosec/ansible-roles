Role: Common
=========

This role performs basic setup common to most hosts within our infrastructure.

Requirements
------------

The internal CA certificate file needs to be copied to files/cacert.pem.

Role Variables
--------------

Variables relating to the internal YUM repository:

repo:
  name      - Repository name
  baseurl   - Repository base URL
  enabled   - Whether to enable the repository (1 to enable; 0 to disable)
  gpgcheck  - Whether to check GPG signatures
  gpgkey    - Path to GPG public key

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

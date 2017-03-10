# etc-git

Configure a GIT repository in /etc to track configuration changes.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - mbocquet.etc-git

or

    - hosts: servers
      roles:
         - { role: mbocquet.etc-git, x: 42 }

if any variables comes in the future fot this role

License
-------

GPLv3

Author Information
------------------

http://www.sekoya.org

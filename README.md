# gitrepo

Ansible role to configure a GIT repository on targets in a specific folder (for
example in /etc to track configuration changes).

## Requirements

None.

## Role Variables

gitrepo_folder : folder to 'gitify'

gitrepo_dotgitignore : list of files/folders to ignore. This list will be used
to construct .gitignore file

See defaults/main.yml for an example. Variables should not be modified there
but defined elsewhere in group_vars/ of host_vars/ files.

## Dependencies

None.

## Install this role as submodule in a git repository

`git submodule add https://git.sekoya.org/mb/gitrepo.git roles/gitrepo`

## Example Playbook

    - hosts: servers
      roles:
         - gitrepo

or

    - hosts: servers
      roles:
         - { role: gitrepo, gitrepo_folder: '/etc' }

if any variables comes in the future fot this role.

## License

GPLv3

## Author Information

http://www.sekoya.org

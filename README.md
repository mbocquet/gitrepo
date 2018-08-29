# etc-git

Configure a GIT repository in /etc to track configuration changes.

## Requirements

None.

## Role Variables

etc_git_dotgitignore : list of files/folders to ignore.

See defaults/main.yml for an example. This variable should not be modified there but defined elsewhere in group_vars/ of host_vars/ files.

## Dependencies

None.

## Install this role as submodule in a git repository

`git submodule add https://github.com/mbocquet/etc-git.git roles/etc-git`

## Example Playbook

    - hosts: servers
      roles:
         - etc-git

or

    - hosts: servers
      roles:
         - { role: etc-git, x: 42 }

if any variables comes in the future fot this role.

## License

GPLv3

## Author Information

http://www.sekoya.org

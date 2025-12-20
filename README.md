# Ansible gedit role

[![Alma9-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/alma9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/alma9-ci-caller.yml) [![Rocky9-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/rocky9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/rocky9-ci-caller.yml) [![CentOSStream9-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/centosstream9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/centosstream9-ci-caller.yml) [![Debian12-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/debian12-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/debian12-ci-caller.yml) [![Ubuntu2204-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/ubuntu2204-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/ubuntu2204-ci-caller.yml)

This role includes a full vagrant based molecule testing setup at `molecule/default`

## Deprecated

This role only makes sense with a desktop environment and was tehrefore integrated into this [role](https://github.com/philnewm/ansible-gnome)

## Structure

```code
📦 ansible-gedit
 ┣ 📂 defaults
 ┃ ┗ 📜 main.yml
 ┣ 📂 files
 ┃ ┗ 📜 lavanda.xml
 ┣ 📂 meta
 ┃ ┗ 📜 main.yml
 ┣ 📂 molecule
 ┃ ┗ 📂 default
 ┃   ┗ 📜, 📜, 📜, scenario_files
 ┣ 📂 tasks
 ┃ ┣ 📜 main.yml
 ┃ ┣ 📜 present.yml
 ┃ ┣ 📜 dependencies.yml
 ┃ ┣ 📜 theme.yml
 ┃ ┣ 📜 absent.yml
 ┃ ┗ 📜 init.yml
 ┣ 📂 vars
 ┃ ┗ 📜 main.yml
 ┗ 🗒️ README.md
 ┗ 📓 requirements.txt

```

Describe and explain role structure.

## Requirements

Elaborate external dependencies and how to use them.

## Role Variables

* defaults/main.yml
  * first_var
  * sec_var
  * third_var
* vars/main.yml
  * first_var
  * sec_var
  * third_var

## Dependencies

List role ansible-galaxy dependencies - if any.

## Example Playbook

Add an example playbook

```yaml
---

tasks:
  - name: Include ansible-gedit present
    ansible.builtin.include_role:
      name: ansible-gedit
    vars:
      state: present

...
```

## License

Add license - if any.

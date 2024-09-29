## Role Name

[![Alma9-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/alma9-ci.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/alma9-ci.yml)  [![Debian12-CI](https://github.com/philnewm/ansible-gedit/actions/workflows/debian12-ci.yml/badge.svg)](https://github.com/philnewm/ansible-gedit/actions/workflows/debian12-ci.yml)

Role description

This role includes a full vagrant based molecule testing setup at `molecule/default`

# Structure

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

Ellaborate external dependencies and how to use them.

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
      gedit_state: present

...
```
## License

Add license - if any.

## Changes to role template

* Add github action that flags empty directories on release creation

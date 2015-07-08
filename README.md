<img src="http://www.elao.com/images/corpo/logo_red_small.png"/>

# Ansible Role: Hugo

This role will assume the setup the static site generator: Hugo (http://gohugo.io/) 

It's part of the ELAO Ansible Stack but can be used as a stand alone component for usecase chekout [Manalas project](http://manalas.com).

## Requirements

- Ansible 1.7.2+

## Dependencies

- Golang 1.4.2 (You can use https://github.com/ElaoInfra/ansible-role-apt to install it.)

## Installation

Using ansible galaxy:

```bash
ansible-galaxy install elao.hugo
```
You can add this role as a dependency for other roles by adding the role to the meta/main.yml file of your own role:

```yaml
dependencies:
  - { role: elao.hugo }
```

## Role Variables

|Name|Default|Type|Description|
|----|-------|----|-----------|
| elao_hugo_version| 0.14 | String | Hugo version |


## Example playbook

    - hosts: servers
      roles:
         - { role: elao.hugo }

# Licence

MIT

# Author information

ELAO [**(http://www.elao.com/)**](http://www.elao.com)

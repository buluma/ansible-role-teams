# [Ansible role teams](#teams)

Ansible Role for Microsoft Teams Installation

|GitHub|Version|Issues|Pull Requests|
|------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-teams/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-teams/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-teams.svg)](https://github.com/buluma/ansible-role-teams/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-teams.svg)](https://github.com/buluma/ansible-role-teams/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-teams.svg)](https://github.com/buluma/ansible-role-teams/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from [`molecule/default/converge.yml`](https://github.com/buluma/ansible-role-teams/blob/master/molecule/default/converge.yml) and is tested on each push, pull request and release.

```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - role: buluma.teams
```

The machine needs to be prepared. In CI this is done using [`molecule/default/prepare.yml`](https://github.com/buluma/ansible-role-teams/blob/master/molecule/default/prepare.yml):

```yaml
---
- name: Prepare
  hosts: all
  gather_facts: yes
  become: yes
  serial: 30%

  roles:
    - role: buluma.bootstrap
    - role: buluma.ca_certificates
```

Also see a [full explanation and example](https://buluma.github.io/how-to-use-these-roles.html) on how to use these roles.

## [Role Variables](#role-variables)

The default values for the variables are set in [`defaults/main.yml`](https://github.com/buluma/ansible-role-teams/blob/master/defaults/main.yml):

```yaml
---
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-teams/blob/master/requirements.txt).

## [State of used roles](#state-of-used-roles)

The following roles are used to prepare a system. You can prepare your system in another way.

| Requirement | GitHub | Version |
|-------------|--------|--------|
|[buluma.bootstrap](https://galaxy.ansible.com/buluma/bootstrap)|[![Ansible Molecule](https://github.com/buluma/ansible-role-bootstrap/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-bootstrap/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-bootstrap.svg)](https://github.com/shadowwalker/ansible-role-bootstrap)|
|[buluma.epel](https://galaxy.ansible.com/buluma/epel)|[![Ansible Molecule](https://github.com/buluma/ansible-role-epel/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-epel/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-epel.svg)](https://github.com/shadowwalker/ansible-role-epel)|
|[buluma.ca_certificates](https://galaxy.ansible.com/buluma/ca_certificates)|[![Ansible Molecule](https://github.com/buluma/ansible-role-ca_certificates/actions/workflows/molecule.yml/badge.svg)](https://github.com/buluma/ansible-role-ca_certificates/actions/workflows/molecule.yml)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-ca_certificates.svg)](https://github.com/shadowwalker/ansible-role-ca_certificates)|

## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-teams/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|[Ubuntu](https://hub.docker.com/repository/docker/buluma/ubuntu/general)|all|
|[Kali](https://hub.docker.com/repository/docker/buluma/kali/general)|all|
|[EL](https://hub.docker.com/repository/docker/buluma/enterpriselinux/general)|8|
|[opensuse](https://hub.docker.com/repository/docker/buluma/opensuse/general)|all|
|[Debian](https://hub.docker.com/repository/docker/buluma/debian/general)|all|
|[Fedora](https://hub.docker.com/repository/docker/buluma/fedora/general)|all|

The minimum version of Ansible required is 2.12, tests have been done to:

- The previous version.
- The current version.
- The development version.

If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-teams/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-teams/blob/master/CHANGELOG.md)

## [License](#license)

[Apache-2.0](https://github.com/buluma/ansible-role-teams/blob/master/LICENSE).

## [Author Information](#author-information)

[buluma](https://buluma.github.io/)


### [Special Thanks](#special-thanks)

Template inspired by [Robert de Bock](https://github.com/robertdebock)

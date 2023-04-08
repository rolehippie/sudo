# sudo

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/sudo)
[![General Workflow](https://github.com/rolehippie/sudo/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/sudo/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/sudo/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/sudo/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/sudo/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/sudo/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/sudo)](https://github.com/rolehippie/sudo/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.sudo-blue)](https://galaxy.ansible.com/rolehippie/sudo)

Ansible role to install and configure sudo.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [sudo_env_keep](#sudo_env_keep)
  - [sudo_groups](#sudo_groups)
  - [sudo_secure_path](#sudo_secure_path)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### sudo_env_keep

List of environment to keep

#### Default value

```YAML
sudo_env_keep:
  - LANG
  - LC_ADDRESS
  - LC_CTYPE
  - LC_COLLATE
  - LC_IDENTIFICATION
  - LC_MEASUREMENT
  - LC_MESSAGES
  - LC_MONETARY
  - LC_NAME
  - LC_NUMERIC
  - LC_PAPER
  - LC_TELEPHONE
  - LC_TIME
  - LC_ALL
  - LANGUAGE
  - LINGUAS
  - XDG_SESSION_COOKIE
```

### sudo_groups

List of groups to create and use

#### Default value

```YAML
sudo_groups:
  - admin
  - sudo
  - wheel
```

### sudo_secure_path

List of secure executable paths

#### Default value

```YAML
sudo_secure_path:
  - /usr/local/sbin
  - /usr/local/bin
  - /usr/sbin
  - /usr/bin
  - /sbin
  - /bin
  - /usr/X11R6/bin
  - /snap/bin
```

## Discovered Tags

**_sudo_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)

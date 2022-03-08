# sudo

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/sudo) [![Testing Build](https://github.com/rolehippie/sudo/workflows/testing/badge.svg)](https://github.com/rolehippie/sudo/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/sudo/workflows/readme/badge.svg)](https://github.com/rolehippie/sudo/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/sudo/workflows/galaxy/badge.svg)](https://github.com/rolehippie/sudo/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/sudo)](https://github.com/rolehippie/sudo/blob/master/LICENSE)

Ansible role to install and configure sudo.

## Sponsor

[![Proact Deutschland GmbH](https://proact.eu/wp-content/uploads/2020/03/proact-logo.png)](https://proact.eu)

Building and improving this Ansible role have been sponsored by my employer **Proact Deutschland GmbH**.

## Table of content

- [Default Variables](#default-variables)
  - [sudo_env_keep](#sudo_env_keep)
  - [sudo_groups](#sudo_groups)
  - [sudo_secure_path](#sudo_secure_path)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

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

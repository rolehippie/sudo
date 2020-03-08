# sudo

[![Build Status](https://cloud.drone.io/api/badges/rolehippie/sudo/status.svg)](https://cloud.drone.io/rolehippie/sudo)

Ansible role to configure sudo

## Table of content

* [Default Variables](#default-variables)
  * [sudo_env_keep](#sudo_env_keep)
  * [sudo_groups](#sudo_groups)
  * [sudo_secure_path](#sudo_secure_path)
* [Dependencies](#dependencies)
* [License](#license)
* [Author](#author)

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

## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)

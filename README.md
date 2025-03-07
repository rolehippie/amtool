# alertmanager

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/amtool)
[![General Workflow](https://github.com/rolehippie/amtool/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/amtool/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/amtool/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/amtool/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/amtool/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/amtool/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/amtool)](https://github.com/rolehippie/amtool/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.amtool-blue)](https://galaxy.ansible.com/rolehippie/amtool)

Ansible role to install Alertmanager CLI.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [amtool_download](#amtool_download)
  - [amtool_extract_directory](#amtool_extract_directory)
  - [amtool_group](#amtool_group)
  - [amtool_install_directory](#amtool_install_directory)
  - [amtool_owner](#amtool_owner)
  - [amtool_version](#amtool_version)
  - [amtool_version_changed](#amtool_version_changed)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### amtool_download

URL to the archive of the release to install

#### Default value

```YAML
amtool_download: https://github.com/prometheus/alertmanager/releases/download/v{{
  amtool_version }}/alertmanager-{{ amtool_version }}.linux-amd64.tar.gz
```

### amtool_extract_directory

Directory in which to extract the downloaded archive

#### Default value

```YAML
amtool_extract_directory: /usr/local/src
```

### amtool_group

Group who will own the binary file

#### Default value

```YAML
amtool_group: root
```

### amtool_install_directory

Directory in which to install the binary

#### Default value

```YAML
amtool_install_directory: /usr/bin
```

### amtool_owner

User who will own the binary file

#### Default value

```YAML
amtool_owner: root
```

### amtool_version

Version of the release to install

#### Default value

```YAML
amtool_version: 0.28.1
```

### amtool_version_changed

Fact to define if the version has changed

## Discovered Tags

**_amtool_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)

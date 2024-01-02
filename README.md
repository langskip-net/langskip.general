<div align="center"> <img src="./static/img/logo_langskip.png"/ width=40%> </div>

# Ansible Collection - General

![Button: GPL v3](https://img.shields.io/badge/License-GPLv3-green.svg)
![Version](https://img.shields.io/badge/Version-1.0-blue.svg)
![Button: Template](https://img.shields.io/badge/Projet-Ansible-red.svg)

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
   - 2.1 [Dependencies](#dependencies)
   - 2.2 [Installation](#installation)
   - 2.3 [Usage](#usage)
3. [Additional Documentation](#Additional_Documentation)
3. [About](#about)
4. [Contributions](#contributions)
5. [License](#license)

## Introduction

This repository contains resource for automating various tasks within the Langskip.net Platform.

## Getting Started
### Dependencies

Before you begin, ensure you have the following prerequisites:
- `Ansible` installed on your ansible host.

### Installation

#### Using Command Line Interface (CLI)

  - To install this Ansible collection using the command line interface, follow these steps:
```bash
ansible-galaxy collection install git+https://git.langskip.net/99-public/01-ansible/collections/langskip.general,latest

#### Using a Requirements File

 1. Create a file named requirements.yml.
 2. Add the following content to the equirements.yml file:

```yaml
 collections:
  - name: git+https://git.langskip.net/99-public/01-ansible/collections/langskip.general
    type: git
    version: latest
```

  * Install the collection by running the following command:

```bash
ansible-galaxy collection install -r requirements.yml
```

### Usage

 * To use the collection in your Ansible playbooks, include it like this:

```yaml
---
- name: Example Playbook
  hosts: localhost
  tasks:
    - name: Include role from langskip
      import_role:
        name: langskip.general.<role>
```

## Additional Documentation

For more detailed documentation, including advanced usage and customization options, please refer to the [docs](docs/) folder in this repository.

## About

**Author:** Mahel 'Helphy' Brossier

**Creation date:** December 31, 2023 

**Last Release:** December 31, 2023


## Contributions

Specify how team members or the community can contribute to the project. Provide guidelines on submitting issues, feature requests, and code proposals.

## License

This project is licensed under the [GNU General Public License v3.0 (GPL-3.0)](LICENSE). Refer to the [LICENSE](LICENSE) file for more details.
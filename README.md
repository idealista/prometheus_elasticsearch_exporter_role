# Prometheus Elasticsearch Exporter Ansible role
![Logo](logo.gif)

[![Build Status](https://travis-ci.com/idealista/prometheus_elasticsearch_exporter_role.png)](https://travis-ci.com/idealista/prometheus_elasticsearch_exporter_role)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-idealista.prometheus_elasticsearch_exporter_role-B62682.svg)](https://galaxy.ansible.com/idealista/prometheus_elasticsearch_exporter_role)



This ansible role installs [Prometheus Elasticsearch Exporter](https://github.com/prometheus-community/elasticsearch_exporter) in a Debian environment. It has been tested for the following Debian versions:

* Bullseye

This role has been generated using the [cookiecutter](https://github.com/cookiecutter/cookiecutter) tool, you can generate a similar role that fits your needs using the [cookiecutter template](https://github.com/idealista/cookiecutter-ansible-role).

- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installing](#installing)
- [Usage](#usage)
- [Testing](#testing)
- [Built With](#built-with)
- [Versioning](#versioning)
- [Authors](#authors)
- [License](#license)
- [Contributing](#contributing)

## Getting Started
These instructions will get you a copy of the role for your Ansible playbook. Once launched, it will install Elasticsearch Exporter in a Debian system.

### Prerequisites

Ansible >= 4 version installed.

Molecule >= 4 version installed.

For testing purposes, [Molecule](https://molecule.readthedocs.io/) with [Docker](https://www.docker.com/) as driver and [Goss](https://github.com/aelsabbahy/goss) as verifier.

### Installing

Create or add to your roles dependency file (e.g requirements.yml):

```
- src: idealista.prometheus_elasticsearch_exporter_role
  version: 1.1.0
  name: prometheus_elasticsearch_exporter_role
```

Install the role with ansible-galaxy command:

```
ansible-galaxy install -p roles -r requirements.yml -f
```

Use in a playbook:

```
---
- hosts: someserver
  roles:
    - role: prometheus_elasticsearch_exporter_role
```

## Usage

Look to the [defaults](defaults/main.yml) properties file to see the possible configuration properties, it is very likely that you will not need to override any variables.


## Testing

### Install dependencies

```sh
$ pipenv sync
```

For more information read the [pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/).

### Test

```sh
$ pipenv run molecule test 
```

## Built With

![Ansible](https://img.shields.io/badge/ansible-10.5.0-green.svg)
![Molecule](https://img.shields.io/badge/molecule-24.9.0-green.svg)
![Goss](https://img.shields.io/badge/goss-0.3.18-green.svg)

## Versioning

For the versions available, see the [tags on this repository](https://github.com/idealista/prometheus_elasticsearch_exporter_role/tags).

You can see what change in each version in the [CHANGELOG.md](CHANGELOG.md) file.

## Authors

* **Idealista** - *Work with* - [idealista](https://github.com/idealista)

See also the list of [contributors](https://github.com/idealista/prometheus_elasticsearch_exporter_role/contributors) who participated in this project.

## License

![Apache 2.0 License](https://img.shields.io/hexpm/l/plug.svg)

This project is licensed under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license - see the [LICENSE](LICENSE) file for details.

## Contributing

Please read [CONTRIBUTING.md](.github/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

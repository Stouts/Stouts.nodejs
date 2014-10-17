Stouts.nodejs
=============

[![Build Status](https://travis-ci.org/Stouts/Stouts.nodejs.png)](https://travis-ci.org/Stouts/Stouts.nodejs)

Ansible role which manage nodejs and npm packages.

#### Requirements

Only tested on ubuntu for now.

#### Variables

```yaml
nodejs_enabled: yes                       # The role is enabled

nodejs_repository: ppa:chris-lea/node.js  # NodeJS PPA
nodejs_npm_modules: []                    # List modules which will be installed
```

#### Usage

Add `Stouts.nodejs` to your roles and set vars in your playbook file.

Example:

```yaml

- hosts: all

  roles:
    - Stouts.nodejs

  vars:
    nodejs_npm_modules:
      - bower
      - jshint
```

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Stouts/Stouts.nodejs/issues)!

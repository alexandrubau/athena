
This repository is used as a boilerplate to help you get going to what you love the most: coding.

## How to use

Just clone this repository and copy all its contents (without the `.git` folder) into your future project folder. Navigate to `auto` folder and run `vagrant up` to start the engine.

## How to configure

As you may have noticed, by default it installs only `apache` and `vagrant` roles. But feel free to install other roles by uncommenting lines from `auto/provision.yml`.

Each role can be configured individually by using parameters. All parameters should be specified in `auto/inventories/dev/group_vars/all.yml`. You can check all available parameters in the list of roles below.

## List of roles:
- [Core](https://github.com/alexandrubau/ansible-core)
- [Adminer](https://github.com/alexandrubau/ansible-adminer)
- [Apache](https://github.com/alexandrubau/ansible-apache)
- [Deploy](https://github.com/alexandrubau/ansible-deploy)
- [MySQL](https://github.com/alexandrubau/ansible-mysql)
- [Node.js](https://github.com/alexandrubau/ansible-nodejs)
- [PHP](https://github.com/alexandrubau/ansible-php)
- [Samba](https://github.com/alexandrubau/ansible-samba)
- [Vagrant](https://github.com/alexandrubau/ansible-vagrant)
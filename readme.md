
## Welcome

This repository is used as a boilerplate to help you get going to what you love the most: coding.

## How to use

Just clone this repository and copy all its contents (without the `.git` folder) into your future project folder. Navigate to `auto` folder and run `vagrant up` to start the engine.

## How to configure

As you may have noticed, by default it installs only `apache` and `vagrant` roles. But feel free to install other roles by uncommenting lines from `auto/provision.yml`.

Each role can be configured individually by using parameters. All parameters should be specified in `auto/inventories/dev/group_vars/all.yml`. You can check all available parameters in the list of roles below.

## List of roles:
- [Core](https://github.com/alexandrubau/ansible-core)
- [ACL](https://github.com/alexandrubau/ansible-acl)
- [Adminer](https://github.com/alexandrubau/ansible-adminer)
- [Apache](https://github.com/alexandrubau/ansible-apache)
- [Deploy](https://github.com/alexandrubau/ansible-deploy)
- [MySQL](https://github.com/alexandrubau/ansible-mysql)
- [Nginx](https://github.com/alexandrubau/ansible-nginx)
- [NodeJS](https://github.com/alexandrubau/ansible-nodejs)
- [PHP](https://github.com/alexandrubau/ansible-php)
- [Samba](https://github.com/alexandrubau/ansible-samba)
- [Vagrant](https://github.com/alexandrubau/ansible-vagrant)

## Frequently asked questions

**Where do I put my application logic?**  
After you installed all the necessary roles, you might  also have to do something specific for some frameworks such as: running migrations, copying templates, etc. Feel free to put your custom Ansible tasks in `auto/roles/app/tasks/main.yml` and include the `app` role. The `app` role should be placed last.

## How to contribute

Feel free to make pull requests if you want to share the knowledge or open issue tickets if you found any bugs or you wish for improvements.

## Coding guidelines for roles

- Role name must be specific and very simple;
- It must follow the conventional directory structure;
- All parameters must start with the role name;
- All "private" parameters must start with `_`;
- Make sure your tasks are run only if needed;
- Allow the user to lock the version of the package;
## aks.ansible-users

This role can be used to manage user accounts and groups. You can
manage almost all aspects of the users' account, like UID/GID, home
directory, shell, etc. 

Accounts are configured using lists in Ansible inventory, with lists (single or
separate) for:

* admin accounts;
* global list of users created on each host in a cluster;
* list of users created on a group of hosts;
* list of users created on a specific host;
* a single global list of users can have a 'hosts' specifier, limiting
  the management of that user to the named hosts;
* ssh keys can be managed with actual key content, or with named files;
* the source ssh key files can have explicit path names, or be named 
  relative to a common directory path `user_keyfiles_dir`.

### Installation

This role requires at least Ansible `v1.7.0`. To install it, run:

    ansible-galaxy install aks.ansible-users

### Documentation

### Authors and license

`ansible-users` role was originally written by:
- Maciej Delmanowski | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)

It has been forked and augmented by:
- Alan Stebbens | [email](mailto:aks@stebbens.org) | [Twitter](https://twitter.com/aks_sba) | [Github](https://github.com/aks)

License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)


# ansible-plays-tl

Ansible playbook for the [JVM Development Environment](https://github.com/kurron/jvm-development-environment)
to install both common use and development related tools for my workspace at Transparent Language.

The JVM Development Environment created by @kurron already provides many helpful tools and software.
I've also created privately used in-house, team specific playbooks for provisioning environments.
These plays are more generally targeted, and allow for more comfortable use of the vagrant box.

## Roles

This playbook uses roles for modularity.

#### Common

* Install file-roller (xfce4 compatible archive manager).
* Install httpie (cli http tool).
* Install gedit (gui text editor).
* Install gyazo screen capture.
* Install plank (osx drawer)

#### Development

* Install python dev libs.
* Install docker-compose.
* Install aws-cli.
* Install mongodb compass.
* Install sqlectron.
* Install vs-code themes and extensions (Python/Web).

## Use

These plays should be ran by @kurron's vagrant script, simply export `USER_PLAYS` as `https://github.com/neetjn/ansible-plays-tl.git`
prior to running `vagrant up` to create your box.

---
Copyright (c) 2018 John Nolette Licensed under the MIT license.

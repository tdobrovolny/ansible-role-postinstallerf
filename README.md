[![Build Status](https://travis-ci.org/tdobrovolny/ansible-role-postinstallerf.svg?branch=master)](https://travis-ci.org/tdobrovolny/ansible-role-postinstallerf)

PostinstallerF
==============

Add repository and install postinstallerf from https://github.com/kuboosoft/postinstallerf.

PostInstallerF will install all the software that Fedora doesn't include commonly, after running Fedora for the first time. Its easy for a new user. PostInstallerF contains everything that you need for your daily computing. More and actual info you found on https://github.com/kuboosoft/postinstallerf

Requirements
------------

 - ansible assert module
 - ansible command module
 - ansible get_url module
 - ansible package module
 - ansible rpm_key module

Role Variables
--------------

This role does not use settable variables.

Dependencies
------------

This role does not depend on any role.

Example Playbook
----------------

    - hosts: workstations
      roles:
         - { role: tdobrovolny.postinstallerf, when: ansible_distribution == "Fedora" }

License
-------

GPL v 3

Role Author Information
-----------------------

Tomas Dobrovolny - sdobrtomas@gmail.com - https://github.com/tdobrovolny


PostinstallerF Author Information
---------------------------------

Author of PostinstallerF repo, package and software is https://github.com/kuboosoft and GitHub repo https://github.com/kuboosoft/postinstallerf
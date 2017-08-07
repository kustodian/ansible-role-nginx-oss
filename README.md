Ansible NGINX OSS Role
======================

[![Build Status](https://travis-ci.org/nginxinc/ansible-role-nginx-oss.svg?branch=master)](https://travis-ci.org/nginxinc/ansible-role-nginx-oss)

This role installs NGINX OSS on your target host. It supports most CentOS/RHEL/Debian/Ubuntu/SLES distributions.

Requirements
------------

This role was developed using Ansible 2.3.1.0 and as such might not work if a previous version of Ansible is employed.

The following platforms have been tested and are oficially supported:

    CentOS:
      versions:
        - 6
        - 7
    RedHat:
      versions:
        - 6
        - 7
    Debian:
      versions:
      - jessie
      - stretch
    Ubuntu:
      versions:
      - trusty
      - xenial
      - yakkety
    SUSE/SLES:
      versions:
        - 12

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

This is a sample playbook file for deploying NGINX OSS from within an online cloud provider.

    ---
    - hosts: localhost
      remote_user: root
      become: true
      roles:
        - role: ansible-nginx-oss

This is a sample playbook file for deploying NGINX OSS to a dynamic inventory containing the `nginx` tag.

    ---
    - hosts: tag_nginx
      remote_user: root
      become: true
      roles:
        - role: ansible-nginx-plus

License
-------

Simplified BSD License

Author Information
------------------

Alessandro Fael Garcia

**NGINX Inc**

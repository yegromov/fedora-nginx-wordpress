

# WordPress Ansible for Fedora 38 using nginx and mariadb

This repository contains a playbook for installing the latest version of Wordpress in Fedora 38 including:

* nginx installation
* mariaDB installation
* Wordpress installation
* SELinux configuration
* firewalld configuration

Please note that SELinux will prevent installing any update, you need to disable it (or relabel to httpd_sys_rw_content_t) during maintenance

## Usage

Edit values in `vars/` directory

Run:

`ansible-playbook -i hosts.yml wordpress.yml`

## Note
The current implementatins has been created for demo purposes, so nginx will serve just using http on 80/tcp port

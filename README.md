# vagrant-laravel
A Vagrant box that provisions PHP 7, Nginx, Percona MySQL 5.7 for use with Laravel.

## How to Use
* Install Vagrant
* vagrant up
* vagrant ssh
* cd /apps && laravel new app

By default, Nginx serves /apps/app/public.

## Variables
Variables can be found in ./php-provisioner/roles/provisioner/vars/main.yml

SQL_DATABASES
  A list of databases to create.

SQL_USERS
  A list of users and permissions to create.

LARAVEL_PROJECT_NAME
  This is the name of the project.  If unset, it will use "app" by default.

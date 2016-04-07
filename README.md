# vagrant-laravel
A Vagrant box that provisions PHP 7, Nginx, Percona MySQL 5.7 for use with Laravel.

## How to Use
* Install Vagrant
* vagrant up
* vagrant ssh
* cd /apps && laravel new app

By default, Nginx serves /apps/app/public.

## Extra Variables
Extra variables can be found in ./php-provisioner/roles/provisioner/vars/main.yml

SQL_DATABASES
  A list of databases to create.

SQL_USERS
  A list of users and permissions to create.

LARAVEL_PROJECT_NAME
  This is the name of the project.  If unset, it will use "app" by default.

## Non-Commit Variables

Non-commit variables can be found in ./php-provisioner/roles/provisioner/vars/non-commit.yml

By default, changes to these files WILL NOT be committed to git.

GITHUB_API_TOKEN
  If you want to define a Github API token to prevent issues with the install process, you can set the value here.  If no value is set and it is required, it will prompt you during the installation.

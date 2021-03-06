# Vagrant LEMP-stack

Easily configurable local LEMP-environment for multiple hostnames.

### What's included?
* [nginx](https://nginx.org/en/)
* [MySQL](https://www.mysql.com/)
* [php7](http://php.net/manual/en/migration70.new-features.php)
* [php-fpm](https://php-fpm.org/)
* [Ruby 2.3](https://www.ruby-lang.org/en/)
* [oh-my-zsh](http://ohmyz.sh/)
* [Nvm](https://github.com/creationix/nvm)
* [Yarn](https://yarnpkg.com)
* [WP-CLI](http://wp-cli.org/)
* [MailCatcher](https://mailcatcher.me/)

### Getting started

* Install [Vagrant](https://www.vagrantup.com/) & [VirtualBox](https://www.virtualbox.org/wiki/VirtualBox)
* Install [Ansible](http://docs.ansible.com/ansible/intro_installation.html)
* Install hostsupdater-plugin for vagrant: `vagrant plugin install vagrant-hostsupdater`
* Make sure your `ssh-agent` is running and has your SSH keys added to it
  * Autostart `ssh-agent` on shell startup: https://help.github.com/articles/working-with-ssh-key-passphrases/#auto-launching-ssh-agent-on-git-for-windows
* Run `vagrant up`

### Adding sites (projects)
* Add site-information to `config.yml` `sites`-array.
* Run `vagrant provision` to automatically add necessary information to the box & to you hosts-file.

### What if I run into problems...?
* Installing Mailcatcher has been disabled in `/provision/roles/tools/tasks/main.yml` for the time being, since it keeps failing

Like always, you should as Niklas as he knows everything.


![niklas](http://testi.in/niklas.gif "Niklas knows everything")
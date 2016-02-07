# vagrant-python

This is a simplification of the Vagrant file of Allisson Azevedo https://github.com/allisson/vagrant-python-machine

Features:

* Nginx
* Nodejs
    * grunt/gulp/bower
* PostgreSQL
* Python 2.6/2.7/3.2/3.3/3.4/3.5/pypy
* Ruby 1.9.1/1.9.3/2.0/2.1/2.2
    * sass/compass
* Supervisor
* MongoDB


## Requirements

* Virtualbox
* Vagrant
* Ansible

## Installation

```
vagrant plugin install vagrant-vbguest
```

```
vagrant plugin install vagrant-bindfs
```

```
git clone https://github.com/daniellbastos/vagrant-python.git
cd vagrant-python
vagrant up
```



## PostgreSQL

* User: vagrant
* Password: vagrant
* Host: localhost
* Port: 5432


Connect to database:

```
psql template1 -U vagrant -h localhost
```

## Nginx

* Host: 192.168.33.10 (private_network ip)
* Port: 80
* Mapped port: localhost:8000 -> 192.168.33.10:80


## MongoDB

* Host: localhost
* Port: 27017

docker-ce
=========

Installs the latest version of docker ce from the docker repository.

By default, docker-compose is also installed. This can be disabled by passing install_docker_compose = false.

Requirements
------------

There are number of prerequisites for the docker engine that are installed by this role. The list can be found on the docker installation pages:

https://docs.docker.com/install/linux/docker-ce/centos/


Role Variables
--------------
install_docker_compose - true or false
Option to install docker-compose, default is true.

Example Playbook
----------------
The following example will install docker on the localhost

---
  - hosts: 127.0.0.1
    connection: local
  
    tasks:
      - include_role:
          name: docker-ce
...

License
-------

Free

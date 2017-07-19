[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

Docker registry  Role
===================

Install the docker registry and creates the certificates required(recipe for EC3)

Role Variables
--------------

These are the variables that can be passed to this role:

	docker_type_of_node: "front"
	country: "ES"
	region: "Valencia"
	city: "Valencia"
	organization: "UPV"
	ounit: "I3M"
	front_hostname: ""

Example Playbook
----------------
```
  - hosts: server
  roles:
  - { role: 'grycap.docker-registry' }
```
```
  - hosts: client
  roles:
  - { role: 'grycap.docker-registry', front_hostname: 'servername', docker_type_of_node: 'wn' }
```

Contributing to the role
========================
In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.  
Thanks

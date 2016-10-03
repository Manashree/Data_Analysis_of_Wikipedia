=====================================================
MongoDB Ansible Role
=====================================================

1. create a new Ansible role with mongodb as role name
2. Add the MongoDB public GPG key from: hkp://keyserver.ubuntu.com:80 with EA312927 as MongoDB public GPG Key ID when Ubuntu package management imports a key (apt-key)
3. Install mongodb-org with 3.2 Community Edition for Ubuntu Trusty 14.04 LTS by adding a MongoDB repository from: deb http://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.2 multiverse
4. Define the following ansible variables in defaults directory: 
    - mongodb_keyserver (to store hkp://...)
    - mongodb_gpgkey_id (to store EA312...)
    - mongodb_repository_list (to store deb http://...)
    - monogodb_package_name (use ‘mongodb’)
5. Define two handlers: 
    - one for starting mongodb
    - one for restarting mongodb
6. Locate a service file where:
    - destination is /lib/systemd/system/mongodb.service
    - owner/group of the destination file is root
    - mode of the file is 0644
    - reload mongodb after adding this file to remote

""""""""""""""""""
Useful links
""""""""""""""""""
    - http://bdossp-spring2016.readthedocs.io/en/latest/hw5.html 
    - Ansible Basic: http://bdossp-spring2016.readthedocs.org/en/latest/lesson/ansible.html
    - Ansible Playbook: http://bdossp-spring2016.readthedocs.org/en/latest/lesson/ansible_playbook.html
    - Ansible Role: http://bdossp-spring2016.readthedocs.org/en/latest/lesson/ansible_roles.html
    - Ansible Best Practices: https://docs.ansible.com/ansible/playbooks_best_practices.html
    - Ansible official documentation: http://docs.ansible.com/ansible/index.html

Role Name
=========
MongoDB Ansible Role

Requirements
------------
None

Role Variables
--------------
* mongodb_keyserver (Server for GPG key)
* mongodb_gpgkey_id (MongoDB public GPG Key ID when Ubuntu package management imports an apt-key)
* mongodb_repository_list (Installs mongodb-org with 3.2 Community Edition)
* monogodb_package_name (Uses ‘mongodb’ which is the username)
* dest_path (To locate the mongodb service file)
* lock_file_parent (To change ownership of the folder which contains the lock file needed while starting service as a 'mongodb' user)


Dependencies
------------
None

Example Playbook
----------------
    ---
    - hosts: servers
      remote_user: root
      roles:
       - mongodb
License
-------
Apache License

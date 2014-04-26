java
========

Ansible role which installs a server jre or jdk

Requirements
------------

Tested on Anbsible 1.6

Role Variables
--------------
    java_online_install: false             # Whether or not to perform an online installation by downloading the installer
    java_installer_path: /var/installers   # Where to find the installer for an offline installation
    java_version: jre1.7.0_55-x64          # The version of java to install
    java_base_install_dir: /apps           # Where java will be installed
    #java_dist_install: true               # Use native packaging mechanism - Not Implemented

Dependencies
------------

None

Example Playbook
-------------------------

    - hosts: all
      sudo: yes
      roles:
         - java

License
-------

MIT

Author Information
------------------

Jon Hadfield

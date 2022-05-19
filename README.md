RSVP Configuration
=========

Configure RSVP for Junos. (WIP)

Requirements
------------


Role Variables
--------------
rsvp_interfaces: List of Dictionaries containing LDP interfaces and unit
* name: Name of physical interface, string
* unit: unit of interface, int

rsvp_static_paths: List of dictionarys containing data for static RSVP paths
* name: name of static LSP, string
* dest: IP of static path hop, string

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: junos_ldp_config }

License
-------

BSD

Author Information
------------------

Marc Colburn Juniper

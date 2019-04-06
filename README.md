Ansible Role: tamay.confluence
=========

This role installs only [Confluence](https://www.atlassian.com/software/confluence). It does not install and configure a remote database or a reverse proxy. 

Requirements
------------

None.

Role Variables
--------------

List of all variables, including default values.
    
    confluence_version: 6.15.2
    
Version of confluence that should be installed.
    
    confluence_base_dir: /opt/atlassian/confluence

Path where Confluence will be installed.

    confluence_data_dir: /var/atlassian/application-data/confluence

Path where Confluence will keep it's application data.


Dependencies
------------

None.

Example Playbook
----------------

    ---
    
    - hosts: all
    
      vars:
        confluence_version: 6.15.2
    
      roles:
      - tamay.confluence

License
-------

MIT

Author Information
------------------

tamay.mueller@gmail.com
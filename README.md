Role Name
=========

Ansible role to upgrade Jenkins to a specific version

Requirements
------------

Role Variables
--------------

```yaml
# url to get the jenkins war files
jenkins_pkg_url: "https://updates.jenkins-ci.org/download/war"

# jenkins version to which you want to upgrade
jenkins_version: "2.182"
```

Dependencies
------------
Example Playbook
----------------

Example of how to use your role (for instance, with variables passed in as parameters):
```yaml
- hosts: local
    become: true
    roles:
    - ansible-role-jenkins-upgrade
```
License
-------

BSD


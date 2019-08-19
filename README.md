Role Name
=========

Ansible role to upgrade Jenkins to a specific version

Requirements
------------

Role Variables
--------------

```yaml
# url to get the jenkins war files
jenkins_pkg_url: "https://updates.jenkins.io"

# jenkins version to which you want to upgrade
jenkins_version: "2.182"

# jenkins admin password
jenkins_user_password: "<your-password>"

# AWS SSM prefix if password is stored in SSM parameter
jenkins_ssm_prefix: "<your-ssm-parameter-name>"

# jenkins admin user name
jenkins_user_name: "<your-user-name>"

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


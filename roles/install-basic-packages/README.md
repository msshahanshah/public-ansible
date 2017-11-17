### Install basic packages

This role installs the basic packages on a RHEL/CentOS machine. 

The packages currently installed are: epel-release, git, ruby, python, python-setuptools, jq, pip and ansible.

The role also adds trusted CA certificate on the machine as well

To use this role, please add the following in your playbook in the ```roles``` section.

```
    - { role: install_basic_packages }
```



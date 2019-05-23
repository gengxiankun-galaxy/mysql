MySQL
=========

Deploy the MySQL service running under the container via ansible.

Installation
------------

```bash
ansible-galaxy install -p /etc/ansible/roles gengxiankun.mysql
```

Requirements
------------

- CentOS 7.0+
- [Docker](https://github.com/gengxiankun-galaxy/docker)

Role Variables
--------------

| parameter | description |
| --------- | ----------- |
| MYSQL_CONTAINER_NAME | MySQL container name |
| MYSQL_PORT | MySQL port |
| MYSQL_ROOT_PASSWORD | MySQL root password |
| MYSQL_ADMINER_PORT | MySQL adminer port |
| MYSQL_ADMINER_ENBALE | MySQL adminer enbale |
| SRV_PATH | Data persistence base directory |
| OPT_PATH | Service deployment directory |

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - gengxiankun.mysql

License
-------

BSD

Author Information
------------------

This role was created in 2019 by Xiankun Geng, Learn more about the author's role in [galaxy](https://galaxy.ansible.com/gengxiankun).

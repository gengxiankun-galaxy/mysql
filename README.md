MySQL
=========

通过 ansible 部署在容器下运行的 MySQL 服务。

Installation
------------

`ansible-galaxy install gengxiankun.mysql`

Dependencies
------------

- [Docker](https://github.com/gengxiankun-galaxy/docker)

Role Variables
--------------

| parameter | description |
| --------- | ----------- |
| OPT_PATH | 服务部署目录 |
| MYSQL_CONTAINER_NAME | MySQL 容器名称 |
| MYSQL_PORT | MySQL 对外端口 |
| MYSQL_ROOT_PASSWORD | MySQL root 密码 |
| MYSQL_ADMINER_PORT | MySQL adminer 对外端口 |
| MYSQL_ADMINER_ENBALE | 是否启用 MySQL adminer  |
| MYSQL_VOLUME | MySQL 容器数据持久化卷标 |
| MYSQL_VERSION | MySQL Docker 镜像版本 |

Example Playbook
----------------

    - hosts: servers
      roles:
         - gengxiankun.mysql

License
-------

BSD

Author Information
------------------

This role was created in 2019 by Xiankun Geng, Learn more about the author's role in [galaxy](https://galaxy.ansible.com/gengxiankun).

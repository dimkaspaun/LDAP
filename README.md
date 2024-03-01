# LDAP

- Написан Ansible [playbook](./ansible/provision.yml) для конфигурации сервера и клиента
- Настроена аутентификация по SSH-ключам
- Firewall включен на сервере и на клиенте

Развертывание:

```bash
vagant up --no-provision
vagrant provision ipaserver
```

Проверка подключения созданного пользователя:

```bash
vagrant ssh ipaclient 
Last login: Sat Jun 18 17:07:03 2022 from 10.0.2.2
[vagrant@ipaclient ~]$ ssh test_user@localhost
```
![2024-03-01_12-00-21](https://github.com/dimkaspaun/LDAP/assets/156161074/1149de0d-829e-4d1f-b350-1c0150c0a10b)

## Settings

- `pg_password`: the password for the postgresql account.
- `http_host`: your domain name.
- `http_conf`: the name of the configuration file that will be created within nginx.
- `http_port`: HTTP port, default is 80.


## Running this Playbook

Quick Steps:

### 1. Customize Options

```shell
nano vars/default.yml
```

```yml
#vars/default.yml
---
---
http_host: "host"
http_conf: "host.conf"
http_port: "80"
pg_user: "postgres"
pg_password: "postgres"
pg_database: "postgres"
ansible_become_password: "password"
```

### 2. Run the Playbook

```command
ansible-playbook -l [target] -i [inventory file] -u [remote user] playbook.yml
```

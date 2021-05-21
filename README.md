# Ansible Playbook to setup Ubuntu Server

- syntax check

```shell
ansible-playbook -i ./inventory/target.yml site.yml -vv --syntax-check
```

- dry run

```shell
ansible-playbook -i ./inventory/target.yml site.yml -vv --check
```

- run

```shell
ansible-playbook -i ./inventory/target.yml site.yml -vv
```

- run from the middle

```shell
ansible-playbook -i ./inventory/target.yml site.yml -vv --start-at="<task name>"
```

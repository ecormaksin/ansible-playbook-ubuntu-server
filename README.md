# Ansible Playbook to setup Ubuntu Server

```shell
# playbookのシンタックスチェック
ansible-playbook -vv --syntax-check -i ./inventory.yml --extra-vars @control-node.yml --extra-vars @extra-vars.yml site.yml

# ドライラン
ansible-playbook -vv --check -i ./inventory.yml --extra-vars @control-node.yml --extra-vars @extra-vars.yml site.yml

# 実際に実行
ansible-playbook -vv -i ./inventory.yml --extra-vars @control-node.yml --extra-vars @extra-vars.yml site.yml

# 途中から実行
ansible-playbook -vv -i ./inventory.yml --extra-vars @control-node.yml --extra-vars @extra-vars.yml --start-at="<途中から開始したいタスク名>" site.yml
```

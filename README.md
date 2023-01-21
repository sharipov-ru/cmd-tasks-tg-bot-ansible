# cmd-tasks-tg-bot-ansible

Ansible playbook to run https://github.com/sharipov-ru/cmd-tasks-tg-bot

## Usage

### Configure local ENV variables on management machine

Add:

```bash
export CMD_TASKS_TG_BOT_TOKEN=value
export CMD_TASKS_REDIS_URL=value
```

to `.bashrc` or `.zshrc`

### Create & edit inventory file

```bash
cp inventory.yaml.sample inventory.yaml
```

Set `ansible_host` and `ansible_ssh_user` (See https://docs.ansible.com/ansible/latest/inventory_guide/intro_inventory.html) 

### Run ansible

```bash
ansible-playbook -i inventory.yaml playbook.yaml
```





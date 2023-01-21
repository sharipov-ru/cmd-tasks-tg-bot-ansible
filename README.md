### Configure local ENV variables on management machine

export CMD_TASKS_TG_BOT_TOKEN=value
export CMD_TASKS_REDIS_URL=value

### Create & edit inventory file

cp inventory.yaml.sample inventory.yaml

### Run Ansible

ansible-playbook -i inventory.yaml playbook.yaml

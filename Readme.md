# ansible_config
We want to automate the configuration of our workstations using `ansible`. We can do this using playbooks (like [local.yml](local.yml)) to write down all the programs that we want to have installed on our computer. 

To execute this on the localhost machine, we have to install ansible

```console
sudo dnf install ansible
```

and then execute the playbook stored in this git repository

```console
sudo ansible-pull -U https://github.com/mosmuell/ansible_config.git -e"computer_type=<type>"
```

## local.yml
Ansible will execute this playbook by default.

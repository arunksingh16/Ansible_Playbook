# Ansible Playbook

- A playbook is the way to automate tasks in Ansible
- A play is ordered list of tasks

### Validating 

```
ansible-playbook --syntax-check playbook.yml
```

### dry-run

```
ansible-playbook -C playbook.yml
```


### Ad-Hoc Commands

Ad-Hoc command is very helpful in quick tasks.

```
ansible host-pattern -m module -a module_args -i inventory --ask-pass -u remote_user -b(become:yes)

ansible all -m ping
```


### ansibel doc

```
ansible-doc ping

# list all modules
ansible-doc -l
```

### Variables 

- host variable applies to specific host
- group variables applies to all hosts

### Ansible vault

- Ansible provides secure key:value data store
- you can supress output of task as well

```
ansible-vault encrypt secret_file
ansible-vault decrypt secret_file

ansible-playbook playbook.yml --ask-vault-pass
```

### Ansible Facts

- Special Variable that contains information unique to managed host

### Ansible Handlers

- Task respond to notification triggered by other tasks



### Ansible blocks



### Jinja Templates and template module



### Ansibel Roles

- reusable content 


### Ansibel Galaxy

command to manage Ansible roles in shared repositories, the default of which is Ansible Galaxy https://galaxy.ansible.com.

```
# init helps to create a skeleton
ansible-galaxy init users

```

### static and dynamic inventory

# ansible_tutorial

# Git
- git clone git@github.com:FiekBuurman/ansible_tutorial.git
- git config --global user.name "Fiek Buurman"
- git config --global user.email "email@address.now"
- git status
- git add README.md
- git commit -m "updated readme file"
- git push origin main
- git add README.md && git commit -m "updated readme file"
- git add inventory
- git commit -m "first inventory file"

# Ansible
- ansible all --key-file ~/.ssh/ansible -i inventory -m ping
- created ansible.cfg
```
[defaults]
inventory = /home/buurmans/ansible_tutorial/inventory
private_key_file = ~/.ssh/ansible
```
- ansible all -m ping
- ansible all --list-hosts
- ansible all -m gather_facts
- ansible all -m gather_facts --limit 192.168.2.210 
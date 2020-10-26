# ansible-arch
0. Make sure ansible is installed:
```bash
sudo pacman -S ansible
```
1. To install all the roles needed at the same time with one command, run the following:
```bash
ansible-galaxy install -r requirements.yml
```
2. Insert variables to your own liking:
```bash
vim host_vars/localhost.yml
```
3. execute the playbook
```bash
ansible-playbook site.yml
```

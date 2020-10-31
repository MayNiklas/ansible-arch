# ansible-arch
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=lines)](https://github.com/XAMPPRocky/tokei)
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=code)](https://github.com/XAMPPRocky/tokei)
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=files)](https://github.com/XAMPPRocky/tokei)

### Intro
This ansible-playbook is being used for installing Arch Linux on a new computer. Please make sure, that you understand the underlaying roles and what they do before following my quickstart guide. I am NOT responsible to anything that might happen by executing my ansible roles. Generally speaking I want to remind you: doing regular proper backups is a great idea!

### Post install
My arch install is splitted into "pre and postinstall" ansible-playbooks. 
There is a second playbook I'm using to install arch from the live-iso:
[ansible-arch-install](https://github.com/MayNiklas/ansible-arch-install.git)

### Roles used
- [ansible-pacman](https://github.com/MayNiklas/ansible-pacman.git)
- [ansible-arch-keyserver](https://github.com/MayNiklas/ansible-arch-keyserver.git)
- [ansible-arch-xorg](https://github.com/MayNiklas/ansible-arch-xorg.git)
- [ansible-kde-plasma](https://github.com/MayNiklas/ansible-kde-plasma.git)
- [ansible-ssh](https://github.com/MayNiklas/ansible-ssh.git)
- [ansible-ssh-server](https://github.com/MayNiklas/ansible-ssh-server.git)
- [ansible-git](https://github.com/MayNiklas/ansible-git.git)
- [ansible-docker](https://github.com/MayNiklas/ansible-docker.git)
- [ansible-arch-bluetooth-keyboard](https://github.com/MayNiklas/ansible-arch-bluetooth-keyboard.git)
- [ansible-hostname](https://github.com/MayNiklas/ansible-hostname.git)
- [ansible-ufw](https://github.com/MayNiklas/ansible-ufw.git)

### Role Variables:
To be set in group_vars OR host_vars

| Variable       | Description                                  | Default |
|----------------|----------------------------------------------|---------|
|`todo`| todo | `todo` |

### Quick start
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

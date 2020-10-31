# ansible-arch
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=lines)](https://github.com/XAMPPRocky/tokei)
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=code)](https://github.com/XAMPPRocky/tokei)
[![Lines Of Code](https://tokei.rs/b1/github/MayNiklas/ansible-arch?category=files)](https://github.com/XAMPPRocky/tokei)

### Roles used
- [ansible-arch-setup](https://github.com/MayNiklas/ansible-arch-setup.git)
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

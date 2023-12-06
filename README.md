DESCRIPTION

Install Nixos with encrypted btrfs scheme on target device.

HOW TO USE

- Boot a Nixos live environment and connect to the internet
- Install Ansible and git on the live environment
```
nix-shell -p ansible git vim
```
- Clone this repo to the live env
```
git clone https://github.com/parmoli/nixos-install
cd nixos-install
```
- Edit vars.yml to setup variables
```
vim vars.yml
```
- Edit main.yml to comment unnecessary tasks
```
vim main.yml
```
- Run the playbook
```
ansible-playbook main.yml
```
- Install Nixos
```
sudo nixos-install --no-root-passwd
```

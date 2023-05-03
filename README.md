# ansible




# VM Setup 

```
su
usermod -aG sudo microshak

sudo apt update
sudo apt install openssh-server




sudo ufw enable
sudo ufw allow ssh
```


sudo systemctl status ssh
sudo ufw status


# Test
ansible -i ./inventory/hosts ubuntu -m ping --user microshak --ask-pass


## Run a playbook
```ansible
ansible-playbook ./playbooks/apt.yaml --user microshak --ask-pass --ask-become-pass -i ./inventory/hosts

```
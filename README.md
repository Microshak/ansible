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
ansible all -m ping


# Shell
```
ansible master -m shell "lsb_release -a"
```

## Run a playbook
```ansible
ansible-playbook ./playbooks/apt.yaml 
```
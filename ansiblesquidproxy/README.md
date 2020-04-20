### Requirements

* Ansible 2.4.2.0 version 
* Ubuntu 14.04 or Ubuntu 16.04

### İnstall Ansible

```
sudo apt-get update
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

### Edit Ansible hosts

vi /etc/ansible/hosts

```
test
192.168.203.132 ##myLocalIp
```

### ansible-playbook run

ansible-playbook --extra-vars "ip=PROXYIPADDRESS" proxy.yml -kK

### NOTE

###### Squid Proxy Port
> Port : 5353

###### default proxy username password
>admin:admin

###### new password or add user
> htpasswd /etc/squid/squid_passwd username


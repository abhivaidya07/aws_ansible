# ec2_ansible
Here we will create a ec2 instance using Ansible.

##Getting Started

Install pip 
```
$ yum install python-pip -y
```
Install boto for AWS authentication
```
$ pip install boto
```
Create .boto file at $HOME i.e. home directory of user
Add credentials to .boto file
```
$ vi .boto
```
> Note: if you are using a AWS Educate account also copy the token and rename **aws_session_token** to **aws_security_token**

Install Ansible
```
$ yum install ansible
```
Run the playbook
```
$ ansible-playbook task.yml
```

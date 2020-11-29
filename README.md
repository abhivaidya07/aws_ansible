# ec2_ansible
Here we will create a ec2 instance using Ansible.

## Getting Started

## Creating EC2 instance

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
[default]
aws_access_key_id=***
aws_secret_access_key=****
aws_security_token=****
```
> Note: if you are using a AWS Educate account copy the token and rename **aws_session_token** to **aws_security_token**

Install Ansible
```
$ yum install ansible -y
```
Run the playbook
```
$ ansible-playbook ec2.yml
```

## Creating s3 bucket

Install boto3
```
$ pip install boto3
```

Add credentials to .boto file
```
$ vi .boto
[default]
aws_access_key_id=***
aws_secret_access_key=****
aws_security_token=****
```
> Note: if you are using a AWS Educate account copy the token and rename **aws_session_token** to **aws_security_token**

Run the playbook
```
$ ansible-playbook s3.yml
```

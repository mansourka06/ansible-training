# TP4 ansible security

## What is done in this topic :

- **Create a cluster** (1 ansible and 1 client).

- **Create a files directory**, which in turn will contain a secrets directory, which in turn will contain a credentials.vault file

- **Move the admin password variable into this file**

- Next, **encrypt this file** using the ansible-vault encrypt command.

- **Modify the deploy.yml playbook** to instruct it to load the vaulted file as vars_files

- **Generate a key pair** (ssh-keygen -t rsa), leaving all parameters at their default values

- **Copy the contents of the public key** (id_rsa.pub) to the client's /name/admin/.ssh/authorized_host file

- **Modify the inventory file** to add this variable to all hosts ansible_ssh_common_args="-o StrictHostKeyChecking=no

- **Launch your playbook**, adding the parameter that will allow you to supply the vault key

- **Check that all has gone well**


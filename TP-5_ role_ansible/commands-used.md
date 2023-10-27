# Used command for this topic


## Get all roles in requirements.yml file
```bash
ansible-galaxy install -r roles/requirements.yml
```

  OUTPUT
  ```bash
  Starting galaxy role install process
  - extracting ansible-role-containerized-wordpress to /home/vagrant/.ansible/roles/ansible-role-containerized-wordpress
  - ansible-role-containerized-wordpress was installed successfully
  ```


- **The ansible role name is: *ansible-role-containerized-wordpress***


##  Here is an installation of docker-compose 1.29.2 on server1 and server2
  sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
  sudo chmod +x /usr/local/bin/docker-compose
  sudo cp /usr/local/bin/docker-compose /bin/docker-compose
  sudo chmod +x /bin/docker-compose


## Playbook running command :
```bash
ansible-playbook -i hosts --ask-vault-pass wordpress.yml
```
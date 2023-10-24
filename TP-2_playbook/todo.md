# TP2_ansible_playbook

## Description

In this section we are going to write an Ansible playbook that deploy an Apache container using Docker.

## Steps

- Create ansible cluster:  Master(Ansible host) and nodes
- Create the projet directory
- Create the [hosts file](inventory.yml) which contain two groups of servers (dev and prod)
- Write the playbook tasks to deploy Apache in a docker container in inventory servers, using **httpd** image and port **80** to expose the service on internet.
- Install all necessary dependences for the container deployement.
- Verity the playbook synatx using ansible-lint.
- Test the playbook deployment (After the playbook execution, the apache webapp must be available in port 80)

## Playbook execution

```bash
ansible-playbook -i inventory.yml deploy.yml --extra-vars "target_host=dev"
```
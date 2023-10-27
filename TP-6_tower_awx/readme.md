# TP-6_ansible_tower

In this topic, we are deploying tower ansible using docker compose.

## What ansible tower is ?

- Ansible Tower is an enterprise automation platform that enables you to centrally manage and control your Ansible infrastructure and automation workflows. 
- It provides a web-based interface and REST API, making it easier to scale and streamline IT operations. Ansible Tower allows you to schedule, track, and manage Ansible playbooks and roles efficiently. 
- Tower enhances security and collaboration among teams, enabling seamless automation across the entire organization. It serves as the control center for Ansible automation, simplifying complex tasks and accelerating the delivery of applications and services. Ansible Tower is developed and supported by Red Hat.


## Installation Steps

- **Copie docker-compose.yml file to tower home directory:**

```bash
cp docker-compose.yml ~/.awx/awxcompose/
```

- _**Go to tower home directory:**

```bash
cd ~/.awx/awxcompose/
```

- **Start AWX using Docker Compose:**
```bash
docker-compose up -d
```

## Tower Interface

1. **Access**: with our ansible lab ip adress from our navigator (example: 192.168.100.10)

2. **Credentials**: admin/passord


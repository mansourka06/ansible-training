# Used command to deploy the playbook in this topic

## Vaulting the file contianing secret variables
```bash
cd ansible-training/TP-4_security
ansible-vault encrypt security/files/secrets/credentials.yml
```

## Decrypting the file contianing secret variables
```bash
cd ansible-training/TP-4_security
ansible-vault decrypt security/files/secrets/credentials.yml
```

## Running the playbook by asking the vault password
```bash
ansible-playbook -i hosts --ask-vault-pass deploy.yml
```

## Running the playbook without asking the vault password
```bash
ansible-playbook -i hosts deploy.yml
```

## Creating hosts inventory file
```bash
sudo cat << EOF >> /etc/hosts
192.168.99.11   prod-server1.local
192.168.99.12   dev-server1.local
EOF
```

## connexion to servers via ssh
```bash
ssh-copy-id vagrant@prod-server1.local
ssh-copy-id vagrant@dev-server1.local
```

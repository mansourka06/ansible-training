# Commands used for the playbook deployement

## Vaulting the secret variables file
```bash
cd ansible-training/TP-4_security
ansible-vault encrypt security/files/secrets/credentials.yml
```

- command used to decrypt to secret variable file
```bash
cd ansible-training/TP-4_security
ansible-vault decrypt security/files/secrets/credentials.yml
```

## Running the playbook by asking vault password to acces vaulted vars
```bash
ansible-playbook -i hosts --ask-vault-pass deploy.yml
```

## Create inventory hosts file in /etc/hosts
```bash
sudo cat << EOF >> /etc/hosts
192.168.99.11   prod-server1.local
192.168.99.12   dev-server1.local
EOF
```

## Connexion to the servers via ssh
```bash
ssh-copy-id vagrant@prod-server1.local
ssh-copy-id vagrant@dev-server1.local
```

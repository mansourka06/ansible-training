# ad-hoc commands

### ping command
```bash
ansible -i hosts all -m ping
```

### create file command
```bash
ansible -i hosts all -m copy -a "dest=/home/vagrant/toto.txt content='Ansible Training'"
```

### setup command
```bash
ansible -i hosts all -m setup
```

### Calling a variable
```bash
ansible -i inventory server1 -m copy -a "dest=/home/vagrant/toto.txt content='Hello Mansour, Welcome to {{ env }}'"
```
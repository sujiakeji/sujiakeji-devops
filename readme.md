echo '<server-ip> server-001' | sudo tee -a /etc/hosts

ssh-copy-id ubuntu@server-001

ssh-add

sudo vi /etc/ansible/hosts
```
localhost ansible_connection=local ansible_python_interpreter="/usr/bin/env python3"
[server]
server-001 ansible_python_interpreter="/usr/bin/env python3"
```

ansible-playbook -i inventory ubuntu/playbook.yml -bK

ansible-playbook -i inventory python/playbook.yml -bK

ansible-playbook -i inventory java/playbook.yml -bK

ansible-playbook -i inventory git/playbook.yml -bK

ansible-playbook -i inventory docker/playbook.yml -bK

ansible-playbook -i inventory app/playbook.yml -bK

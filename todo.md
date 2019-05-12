hostname revert after reboot

```
sudo sed -i '/preserve_hostname: false/c\preserve_hostname: true' /etc/cloud/cloud.cfg && sudo hostnamectl set-hostname <new-hostname>
```

cloud-init

ansible roles vars location

password encryption, passlib

mysql container exec, link

ubuntu: nvidia, shadowsocks, sogou, idea

docker: nvidia, network, machine, swarm

database: elasticsearch, ceph

operation: jenkins, nginx

frontend: nodejs

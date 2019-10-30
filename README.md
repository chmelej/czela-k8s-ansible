# czela-k8s-ansible

Czela hratky s k8s

- jak zabit existujici cluster
```
ansible-playbook -i hosts.k8s.czela.net 99-destroy-k8s-cluster.yml --ask-become-pass
```
- jak spustit novy cluster
```
ansible-playbook -i hosts.k8s.czela.net 03-init-k8s-cluster.yml --ask-become-pass
```

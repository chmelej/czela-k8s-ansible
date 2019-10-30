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

## TODO
- skript pro vygenerovani roli a namespace
    - kazdy user ma svuj namespace kde muze vsechno a jinak muze jen cist ostatni

- nastaveni NFS, aby bylo mozne sdilet persistentni data mezi nody

- nastaveni ingress, zatim bez https viditelne pouze uvnitr site.
    - vsechno pristupne na domenach *.k8s.czela.net
    - nebudeme resit kolize mezi uzivatelskyma aplikacema (snad se dohodneme)


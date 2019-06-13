# kubespray-ops
  
DevOps Project : Ansible / Kubespray / git submodule / GCP  
Use case : need to create a kubernetes cluster with 3 nodes, 2 slaves and 1 master.
The 3 need etcd.  

```ruby  
> git clone https://github.com/gabyfulchic/kubespray-ops.git
> cd kubespray-ops/
> ansible inventory.ini -m ping
> # only if it answer "pong" so launch the next cmd
> ansible-playbook -i inventory.ini -f cluster.yml
> # then to change kubernetes conf go on a node and edit this
> ~/.kube/config
```

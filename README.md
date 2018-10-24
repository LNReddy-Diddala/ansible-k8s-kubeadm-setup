# ansible-k8s-kubeadm-setup
Create a Kubernetes Cluster Using Kubeadm on CentOS 7

Steps to setup Kubernetes Cluster using these playbooks.

-> Run kube-dependencies.yml playbook to install dependencies on master & node machines.
$ ansible-playbook -i hosts kube-dependencies.yml

-> Run master.yml to launch cluster with necessary settings
$ ansible-playbook -i hosts master.yml

-> Run workers.yml to join worker nodes to the cluster
$ ansible-playbook -i hosts workers.yml

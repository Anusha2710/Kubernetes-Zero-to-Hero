# K8s:

## Docker Vs K8s:

K8s Supports - Cluster(group of nodes)
             - Auto Healing(replica sets, HPA)
             - Auto Healing(API server)
             - Enterprize level Container Orchestration Platform(production level)

## K8s Architechture:

![image](https://github.com/Anusha2710/Kubernetes-Zero-to-Hero/assets/47424821/49d9c7c9-4679-4fc3-b201-c935fe4c5eba)

pod- smallest level of deployment in k8s

- kubelet- creates pod and ensures pod is running, if pod is not running it informs to API server
- container runtime- runs container inside pod
- kubeproxy- provides networking like docker0, generates ip address and load balancing, uses ip tables on linus machines for n/w related configurations

- API server- core component, accepts all incoming requests and exposes k8s to external world, takes decision making on worker nodes
- scheduler- schedules pods or resources on k8s
- etcd - key value stores. stores all info of cluster
- controller manager- manager for k8s inbuilt controllers like relica sets are running or not
- cloud controller manager- manages cluster resources into cloud providers



# CKA (Certified Kubernetes Adminstration)


### Kubernetes: open scource orchristration tools, ensure there is no downtime.


### K8s-Cluster Components:

  1. Master node(control-plane):
     * API-Server: expose k8s api 
     * etcd: key-value store for store deata configraton.
     * schdular: assign pods to spesific node
     * kube-controller manager: compare desired state with current state ,and there are different types of controllers like replication controller, endpoints controller, service account controller and Token controller

  2. Worker node :
     * kubelete : ensure containers are healthy and Ensure pods are running on the nodes
     * k-proxy : Maintains network rules on the nodes to keep SVCs working.
     * container-Runtime : create containers

    


### High Avalibality Cluster :
  * No single point of failure : host should be in different zones
  * kube-apiserver is exposed to worker nodes using a loadbalancer
  * external etcd 



### Terminologies
 * Cluster : Set of connected machines
 * node : singe machine (one of the machines that form the cluster) , Node can be either a **Master** or a **Worker** , Master contains `control plane` components , worker contains **kubelet** which communicates with container runtime
 
 * NameSpaces : logical grouping for Kubernetes objects , Any kubernetes resource uses **default** namespace if no other namespace was specified
 
 * pod : Smallest unit in kubernetes , Each pod can contain **1 or more containers**

 
# CKA (Certified Kubernetes Adminstration)



*Kubernetes: open scource orchristration tools, ensure there is no downtime.*


### K8s-Cluster Components:
    - master node(control-plane):
        - API-Server: expose k8s api 
        - etcd: key-value store for store deata configraton.
        - schdular: assign pods to spesific node
        - kube-controller manager: compare desired state with current state ,and there are different types of controllers like replication controller, endpoints controller, service account controller and Token controller
    - Worker node:
         - kubelete : ensure containers are healthy and Ensure pods are running on the nodes
         - k-proxy : Maintains network rules on the nodes to keep SVCs working.
         - container-Runtime : create containers


* NameSpaces : For grouping Kubernetes objects , Any kubernetes resource uses **default** namespace if no other namespace was specified


* High Avalibality Cluster :
  - No single point of failure : host should be in different zones
  - kube-apiserver is exposed to worker nodes using a loadbalancer
  - external etcd 




* core conseptes in k8s

   - 
  





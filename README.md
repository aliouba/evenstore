
# Prerequisites

Kubernetes Cluster

Kubectl installed and configured

A stoarge class must exist. You d'ont need to setup a new storage class with AKS.

# StatefulSet

The Statefull.yaml file allow to launch 3 evenstore instances (cluster mode). 
You need to customize depending on the storage class and the disk size. For each evenstore instance, a pvc will be created.


# Service

The service.yaml file has two services. 
The first one (es.default.svc.cluster.local) is accessible through the Kube cluser and 
the last one (es-front)  is not required but expose 2113 HTTP PORT to Internet.




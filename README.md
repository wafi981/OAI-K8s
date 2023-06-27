# OAI-k8s
Deploying OAI 5g Core on k8s

# Pre-requisite
The cluster on which these helm charts will be deployed should have RBAC and Multus CNI. Multus is necessary to provide multiple interfaces to AMF and UPF/SPGWU. In case you don't have multus CNI for seconary network interface inside the pod you can still use the ethernet interface provided by the primary CNI. This type of setting is only recommended for playing with rfsimulator. In case you are using minikube or any other Kubernetes deployer make sure you have minimum 4 CPU and 16 GBi of ram.

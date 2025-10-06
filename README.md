###### Author: Lahiru Abeysinghe
##### Last update: 6th October 2025
# Step by Step guide to deploy Canonical Kubernetes on Bare metal


### Read more about [Canonical Kubernetes](https://documentation.ubuntu.com/canonical-kubernetes/release-1.32/)

### In this setup we will use two bare metal servers to deploy Canonical Kubernetes. We also will be using an Virtual machine to deploy Juju controller. (This is optional as Canonical Kubernetes is just a snap installation.) Juju controller allows you to monitor, inspect, and reconfigure your cluster at runtime. By using a Juju controller, you separate Cluster management (handled by Juju) and Cluster operation (done by Kubernetes).

### Below tasks are performed in this lab.

+ Installing OS on baremetal servers and the VM. 
+ Setting up Juju controller
+ Deploying Canonical Kubernetes
+ Integrating local-storage
+ Configuring local container registry
+ External access with ingress-nginx controller

## Setting up bare metal servers and Virtual machine (juju)
### Ubuntu 24.04 LTS will be installed across all the nodes in this lab. 

### This step is pretty much straight forward as no specific configurations are required when installing the OS. 

## Exclusions
+ Configuring Juju HA

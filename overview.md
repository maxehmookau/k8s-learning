# Kubernetes Understanding

## Terms

### k8s

Common abbreviation for Kubernetes. Not something different.

### Cluster

A set of machines (VMs or bare metal) running k8s either as a manager or a worker. Known individually as nodes.

### Node

A manager or a worker machine running k8s as part of a cluster.

### Pod

Runs a container on a k8s cluster. Contains a container (docker), kubelet (which appears to be the bridge between k8s and the pod) as well as a container runtime (like Docker).

### Replication Controller

Set of rules given to a k8s cluster to tell it run a certain number of pods called replicas and make sure that that number keeps running regardless of one of them crashing/stopping.

### Deployment

Deployments are controllers of replication sets (see above) and pods. Can deploy different versions and see deployment history (I think.)

### Service

Provides a private IP address for connecting to containers inside pods. Pods may come and go but the service the containers provide should be available.

### Health Check

Define on a pod how to determine if a pod is healthy. You can define a HTTP endpoint to find out if a pod is healthy.

## Tools

### kubectl

Standard CLI application for managing a k8s cluster.

### kops

CLI tool for managing a kubernetes cluster running on AWS.

### helm

Package manager for k8s cluster?

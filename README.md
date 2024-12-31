# Kubernetes NFS Provisioner 🛠️📦  

This repository provides a Kubernetes deployment setup for an **NFS Provisioner**. It includes YAML configuration files for deploying an NFS Provisioner with necessary resources such as service accounts, roles, StatefulSets, and DaemonSets.

---

## Features ✨  

- **NFS Provisioner**: Dynamically provision NFS-backed persistent volumes in Kubernetes.  
- **YAML Deployment**: Ready-to-use YAML files for easy deployment.  
- **Comprehensive Configuration**: Includes service accounts, RBAC roles, StatefulSets, and DaemonSets.  

---

## Prerequisites 🛠️  

- A running Kubernetes cluster.  
- NFS server accessible to the cluster.  
- `kubectl` configured to access the cluster.  

---

## Installation  

1. Clone the repository:  
git clone https://github.com/your-username/kubernetes-nfs-provisioner.git  
cd kubernetes-nfs-provisioner  

2. Update the `nfs-provisioner-config.yaml` file with your NFS server details:  
```yaml
nfs:
  server: <your-nfs-server-ip>
  path: /exported/path

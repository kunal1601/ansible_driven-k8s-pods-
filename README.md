# 🛠️ Ansible-Driven Configuration Management Inside Kubernetes Pods Using Minikube

This project demonstrates how to run Ansible inside a Kubernetes pod to manage other pods using SSH — all within a **Minikube cluster**.

---

## 📸 Architecture Diagram

![Ansible in Kubernetes using Minikube](./images/ansible-k8s-minikube.png)

---

## 🚀 Project Overview

- **Minikube** is used to create a local single-node Kubernetes cluster.
- Two pods are deployed:
  - 🟡 **Ansible Pod** — acts as the control node
  - 🟢 **Target Pod** (Ubuntu + Nginx + SSH)
- SSH key-based authentication is set up between the pods.
- Ansible is installed inside the Ansible pod and used to manage the target pod.

---

## 🧰 Prerequisites

- Minikube installed (`minikube start`)
- `kubectl` configured to talk to Minikube
- Basic Linux, Ansible & Kubernetes knowledge

---

## 📦 Folder Structure
```
.
├── ansible-pod.yaml
├── nginx-pod.yaml
├── inventory.ini
├── playbook.yml
└── images/
```



# Kubernetes Hands-On Guide

This repository is a **practical guide for learning Kubernetes**. It covers pods, deployments, services, scaling, and self-healing in a single file.

---

## Overview

Kubernetes is an open-source platform for container orchestration. It automates:

- Container deployment and management
- Scaling & load balancing
- Self-healing of applications

Key Concepts:

| Concept    | Description |
|------------|------------|
| Cluster    | Group of nodes running Kubernetes |
| Node       | Single machine in a cluster |
| Pod        | Smallest deployable unit; usually contains one container |
| Deployment | Manages pods; ensures desired number of replicas |
| Service    | Exposes pods internally or externally |
| ReplicaSet | Ensures a specified number of pod replicas are running |

---

## Practical Exercises

### 1. Create a Pod
```bash
kubectl run my-first-pod --image=nginx --restart=Never
kubectl get pods
kubectl describe pod my-first-pod
kubectl logs my-first-pod

# Kubernetes Interview Questions & Answers

## 1. What is Kubernetes? Why is it used?
Kubernetes is an open-source container orchestration platform for automating deployment, scaling, and management of containerized applications. It ensures application reliability, scalability, and efficient resource utilization across clusters.

## 2. What are the core components of Kubernetes architecture?
### Master Node Components:
- **API Server**: Manages the cluster and serves the Kubernetes API.
- **Controller Manager**: Ensures desired states by monitoring and acting on changes.
- **Scheduler**: Allocates Pods to Nodes based on resource requirements.
- **etcd**: A distributed key-value store for cluster data.

### Worker Node Components:
- **Kubelet**: Communicates with the API server and ensures Pods are running.
- **Kube-proxy**: Manages networking and load balancing.
- **Container Runtime**: Runs the containers (e.g., Docker, CRI-O, or containerd).

## 3. Explain the difference between a Pod and a Container.
- **Pod**: The smallest deployable unit in Kubernetes, containing one or more containers.
- **Container**: An isolated runtime environment. Kubernetes manages containers within Pods, not directly.

## 4. What is a Node in Kubernetes?
A Node is a physical or virtual machine that runs Pods and contains necessary components like the **kubelet**, **kube-proxy**, and a **container runtime**.

## 5. What is a Pod in Kubernetes, and why is it considered the smallest deployable unit?
A Pod is a logical group of one or more containers sharing storage, network, and specifications. It is the smallest deployable unit because Kubernetes manages workloads at the Pod level.

## 6. What is a ReplicaSet, and how is it different from a ReplicationController?
- **ReplicaSet**: Ensures a specified number of replicas of a Pod are running. Supports set-based label selectors.
- **ReplicationController**: Similar but supports only equality-based selectors.

## 7. What is the purpose of a Service in Kubernetes?
A **Service** provides a stable network endpoint and load balancing for a set of Pods, abstracting their dynamic IP addresses.

## 8. Explain the concept of Namespaces in Kubernetes.
Namespaces partition cluster resources into isolated segments, enabling multi-tenant environments or resource segmentation.

## 9. What is a Deployment in Kubernetes? How does it manage Pods?
A **Deployment** provides declarative updates for Pods and ReplicaSets, managing scaling, rolling updates, and rollbacks.

## 10. What is the role of etcd in Kubernetes?
**etcd** is a distributed key-value store that stores all cluster data, ensuring consistency and availability for state management.

## 11. Explain ConfigMaps and Secrets. How do they differ?
- **ConfigMaps**: Store configuration data as key-value pairs, not sensitive.
- **Secrets**: Store sensitive data like passwords, encoded in base64 for security.

---
Happy learning! 🚀

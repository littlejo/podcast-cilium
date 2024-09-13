**KCLI Overview**  
KCLI is a tool designed to provide a unified user experience when working with various virtualization platforms (Libvirt, vSphere, AWS, Azure, GCP, IBM Cloud, OpenStack, etc.) and Kubernetes clusters (kubeadm, OpenShift, OKD, k3s, and more). It's highly versatile, offering the ability to manage virtual machines (VMs) and Kubernetes clusters, automate the creation of control planes, and integrate with technologies like HyperShift for hosted control planes.

### Key Features:
- **Unified Management**: Manage VMs and Kubernetes clusters across multiple platforms, such as AWS, GCP, Azure, and OpenShift.
- **Cluster Automation**: Automates the setup of control planes, worker nodes, and other components, with support for kubeadm and OpenShift.
- **HyperShift**: Allows deploying hosted control planes, similar to EKS, making it easy to scale and manage Kubernetes clusters.
- **Predefined Parameters**: You can customize configurations like the number of control planes, node resources, and application setups (e.g., local storage, OpenShift Data Foundation, Multicluster Engine).
- **Integration with Cilium and Network Policies**: KCLI supports Cilium as a network solution, enabling advanced networking and security features for Kubernetes environments.
  
### Example Use Case:
In the demo, the speaker uses a GCP instance with 100GB of RAM and 64 CPUs to showcase the creation of an OpenShift cluster. They demonstrate installing additional components like local storage, Cilium, and HyperShift to handle hosted control planes.

### Workflow:
- **VM Creation**: Use KCLI to create VMs for control planes and workers.
- **Cluster Setup**: Define cluster parameters through a "params" file, including the number of nodes and additional applications.
- **Monitoring**: KCLI provides various commands to monitor and manage VMs, clusters, and Kubernetes operators.
  
### Additional Tools:
- **Console Access**: Direct SSH and serial console access for troubleshooting.
- **Scaling**: Easily scale worker nodes and adjust cluster resources dynamically.
- **Extensibility**: KCLI is highly configurable, allowing users to customize nearly every aspect of VM and cluster creation, from storage to networking.

You can watch the full video here: [https://www.youtube.com/watch?v=Mt5YyO0pRZ8](https://www.youtube.com/watch?v=Mt5YyO0pRZ8)

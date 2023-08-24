# Accessing Kubernetes Clusters using the Teleport Connect Client

You can use the Teleport Connect client to access Kubernetes clusters.

## Prerequisites

- Teleport Connect Client installed on your local machine. See [Installing Teleport Connect Client](/access/teleport/client-installation/) for instructions.
- Kubectl installed on your local machine. See [Installing kubectl](https://kubernetes.io/docs/tasks/tools/#kubectl) for instructions.


## Accessing a Kubernetes Cluster
Launch the Teleport Connect Client and sign in with your account.

Choose the register `Kubes` and select `Connect` to connect to the Kubernetes cluster.

![Teleport Connect K8s](../../assets/images/teleport_connect_k8s.png)

A new terminal window will open with the `kubectl` context set to the Kubernetes cluster.

Now you can run `kubectl` commands to access the Kubernetes cluster.

![Teleport Connect K8s](../../assets/images/teleport_connect_k8s_terminal.png)
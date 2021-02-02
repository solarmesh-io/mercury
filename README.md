# Mercury 

`Mercury` is a tool that install Kubernetes KinD cluster with MetalLB in a few minutes.

![](container.png)

Over years, numerous tools have been developed to provide bootstrap capabilities for a Kubernetes cluster. A considerable proportion of these tools focus on constructing a holistic cluster installation while supplying several flag options for advanced configuration. Undoubtedly, this is the state of the art for when it comes to production-ready clusters, however, these install mechanisms prove to be ponderous and time-consuming for the product development and testing stages. The end-user community required lightweight bootstrap tools to enable speedy and reliable infrastructure provisioning on local environments.

Nowadays, the most prominent tools that simplify the cluster creation on a local machine are minikube, kind, microK8s, k3s, etc. `Mercury` will focus on highlighting kind as a provisioning tool and its advanced configuration to tailor the networking layer. For the sake of simplicity, MetalLB will be the first citizen in this installation.

## Prerequisites

Kind is an open-source tool that generates Kubernetes clusters using Docker. 

The prerequisites is to install `Docker` in your OS.

## Getting started

### Installation

Once `Docker` is installed, all you have to do is to clone this repo and type `./install`

```bash
git clone https://github.com/solarmesh-io/mercury.git
cd mercury
./install
```

### Clean up

When the KinD is no longer needed, you can simply uninstall it

```bash
./uninstall
```

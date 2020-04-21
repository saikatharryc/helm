# HELM charts for Kubernetes

All the charts here provided are ready to launch on Kubernetes using [Kubernetes Helm](https://github.com/helm/helm).

## TL;DR

```bash
$ helm repo add saikatharryc https://saikatharryc.github.io/helm/
$ helm search repo saikatharryc
$ helm install my-release saikatharryc/<chart>
```
## Before you begin


### Install Helm

Helm is a tool for managing Kubernetes charts. Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://github.com/helm/helm#install) and ensure that the `helm` binary is in the `PATH` of your shell.

### Add Repo

The following command allows you to download and install all the charts from this repository:

```bash
$ helm repo add saikatharryc https://saikatharryc.github.io/helm/
```

### Using Helm

Once you have installed the Helm client, you can deploy a saikatharryc Helm Chart into a Kubernetes cluster.

Please refer to the [Quick Start guide](https://github.com/helm/helm/blob/master/docs/quickstart.md) if you wish to get running in just a few commands, otherwise the [Using Helm Guide](https://github.com/helm/helm/blob/master/docs/using_helm.md) provides detailed instructions on how to use the Helm client to manage packages on your Kubernetes cluster.

Useful Helm Client Commands:
* View available charts: `helm search repo`
* Install a chart: `helm install my-release saikatharryc/<package-name>`
* Upgrade your application: `helm upgrade`


### Available Charts:
   - [Judge0](/charts/judge0)
   - [Muescheli](/charts/muescheli)


For any kind of help/issue, please raise [here](https://github.com/saikatharryc/helm/issues).
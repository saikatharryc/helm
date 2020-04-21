muescheli
=========
muescheli antivirus

Current chart version is `18.11.1`

Source code can be found [here](https://github.com/saikatharryc/muescheli)


## Prerequisites

- Kubernetes 1.12+ *
- Helm 2.11+ or Helm 3.0-beta3+ *
- PV provisioner support in the underlying infrastructure (According to the need)

## Installing the Chart

> **NOTE:** You need to [add the helm repository](/README.md#tldr) to perform the below steps.

To install the chart with the release name `my-release`:

```console
$ helm install my-release saikatharryc/muescheli
```

The command deploys Muescheli on the Kubernetes cluster in the default configuration. The [Parameters](#parameters) section lists the parameters that can be configured during installation.

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `my-release` deployment:

For Helm V2:
```console
$ helm delete my-release
```
For Helm V3:
```console
$ helm uninstall my-release
```

The command removes all the Kubernetes components associated with the chart and deletes the release.


## Parameters

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| image.registry | string | `"docker.io"` | Image registry |
| image.repository | string | `"saikatharryc/muescheli"` | Image Repository |
| image.tag | string | `"latest"` | Image Tag |
| service.annotations | string | `nil` | Service annotations done as key:value pairs |
| service.externalTrafficPolicy | string | `"Cluster"` | External Traffic Policy |
| service.nodePorts.http | string | `nil` | Nodepport if available |
| service.port | int | `8091` | HTTP Port |
| service.type | string | `"ClusterIP"` | Service Type (i.e LoadBalancer,NodePort etc) |

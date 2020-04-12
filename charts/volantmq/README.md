volantmq
========
VolantMQ mqtt broker

Current chart version is `0.1.0`





## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| config | string | [config](/charts/volantmq/values.yaml#L147) | The VolantMQ config (for more detailed click config related info [here](https://github.com/VolantMQ/volantmq#config-file) )|
| image.pullPolicy | string | `"IfNotPresent"` | Image repository pull policy  |
| image.registry | string | `"docker.io"` | URL to registry |
| image.repository | string | `"volantmq/volantmq"` | Image repository name  |
| image.tag | string | `"v0.4.0-rc.6"` | Image repository tag  |
| ingress.annotations | object | `{}` | Custom annotations for the ingress (e.g ingress.class ) |
| ingress.enabled | bool | `false` | Enable Ingress Object |
| ingress.extraPaths | list | `[]` | Extra paths to prepend to every host configuration. This is useful when working with annotation based services. |
| ingress.hosts | list | `["chart-example.local"]` | Ingress accepted hostnames |
| ingress.labels | object | `{}` | Custom ingress lavels |
| ingress.path | string | `"/"` | Ingress accepted path |
| ingress.tls | list | `[]` |  |
| livenessProbe.enable | bool | `false` | Enabling Readiness Probe |
| livenessProbe.initialDelay | int | `30` | Intial Delay to take in account |
| livenessProbe.timeout | int | `1` |  Define custom timeout  |
| metrics.enabled | bool | `false` | Enable Service Metrics |
| metrics.serviceMonitor.enabled | bool | `true` | Enable Service Monitor |
| metrics.serviceMonitor.interval | string | `"3s"` | fallback to the prometheus default unless specified |
| metrics.serviceMonitor.namespace | string | `"prometheus"` | Specify a namespace if needed |
| metrics.serviceMonitor.selector.release | string | `"prometheus-operator"` |  prometheus operator release |
| persistence.accessMode | string | `"ReadWriteOnce"` | Define preferred access mode |
| persistence.annotations | object | `{}` | Define PV annotations |
| persistence.enabled | bool | `true` | Enable Persisting data to a persistent volume |
| persistence.size | string | `"8Gi"` | Define volume claim size(default 8GB) |
| readinessProbe.enable | bool | `true` | Enabling Readiness Probe |
| readinessProbe.initialDelay | int | `30` | Intial Delay to take in account |
| readinessProbe.interval | int | `60` | Readiness check interval |
| readinessProbe.timeout | int | `3` |  Define custom timeout  |
| service.annotations | object | `{}` | Kubernetes Service annotations |
| service.clusterIP | string | `"None"` | Kubernetes clusterIp if any |
| service.externalIPs | list | `[]` | Kubernetes Service externalIps |
| service.labels | object | `{}` | Kubernetes Service lavels |
| service.loadBalancerIP | string | `""` | Kubernetes Service LoadBalancerIp |
| service.loadBalancerSourceRanges | list | `[]` | Kubernetes Service Load Balancer source Range |
| service.port | int | `1883` | Kubernetes Service port |
| service.publishNotReadyAddresses | bool | `false` | Kubernetes Service publishNotReadyAddresses |
| service.type | string | `"ClusterIP"` | Kubernetes Service type |
| serviceAccount.create | bool | `false` | Specifies whether a ServiceAccount should be created |
| serviceAccount.name | string | `nil` | The name of the ServiceAccount to use. |
| testFramework.enabled | bool | `true` | Enable Test Framework |
| testFramework.image | string | `"bats/bats"` | Image to be used for testing of the chart |
| testFramework.securityContext | object | `{}` | define securityContext object if any |
| testFramework.tag | string | `"v1.1.0"` | Image Tag for the test framework |


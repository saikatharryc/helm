VolantMQ
========
VolantMQ mqtt broker.

Current chart version is `0.1.0`





## Configuration
The following tables lists the configurable parameters of the VolantMQ chart and their default values.



| Key | Type | Default | Description |
|-----|------|---------|-------------|
| config | string | `"None"` | Override for kubectl default config in the VolantMQ pod(s)|
| image.pullPolicy | string | `"IfNotPresent"` | Image pull policy
 |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"volantmq/volantmq"` |  |
| image.tag | string | `"v0.4.0-rc.6"` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.extraPaths | list | `[]` |  |
| ingress.hosts[0] | string | `"chart-example.local"` |  |
| ingress.labels | object | `{}` |  |
| ingress.path | string | `"/"` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.enable | bool | `false` |  |
| livenessProbe.initialDelay | int | `30` |  |
| livenessProbe.timeout | int | `1` |  |
| metrics.enabled | bool | `false` |  |
| metrics.serviceMonitor.enabled | bool | `true` |  |
| metrics.serviceMonitor.interval | string | `"3s"` |  |
| metrics.serviceMonitor.namespace | string | `"prometheus"` |  |
| metrics.serviceMonitor.selector.release | string | `"prometheus-operator"` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.enabled | bool | `true` |  |
| persistence.size | string | `"8Gi"` |  |
| readinessProbe.enable | bool | `true` |  |
| readinessProbe.initialDelay | int | `30` |  |
| readinessProbe.interval | int | `60` |  |
| readinessProbe.timeout | int | `3` |  |
| service.annotations | object | `{}` |  |
| service.clusterIP | string | `"None"` |  |
| service.externalIPs | list | `[]` |  |
| service.labels | object | `{}` |  |
| service.loadBalancerIP | string | `"None"` |  |
| service.loadBalancerSourceRanges | list | `[]` |  |
| service.port | int | `1883` |  |
| service.publishNotReadyAddresses | bool | `false` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `nil` |  |
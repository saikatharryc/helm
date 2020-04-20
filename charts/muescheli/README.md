muescheli
=========
muescheli antivirus

Current chart version is `18.11.1`

Source code can be found [here](https://github.com/saikatharryc/muescheli)



## Chart Values

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

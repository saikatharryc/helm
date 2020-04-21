[Judge0](https://github.com/judge0/api)
======
Helm implementation of [Judge0](https://github.com/judge0/api) | Free,robust and scalable open-source online code execution system.

Current chart version is `1.0.12`

Default App Version set to `1.5.0`, you can override with values, just like other value/configuration available `values.yaml`.

Source code can be found [here](https://github.com/judge0/api)


## Chart Requirements 
> - If not provided can be configured to automatically spinup thsese

| Repository | Name | Version |
|------------|------|---------|
| https://kubernetes-charts.storage.googleapis.com/ | postgresql | 7.7.2 |
| https://kubernetes-charts.storage.googleapis.com/ | redis | 10.2.0 |


Insta

## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| COUNT | int | `1` |  |
| MAINTENANCE_MODE | bool | `false` |  |
| RAILS_MAX_THREADS | int | `10` |  |
| external.postgresql.host | string | `"localhost"` |  |
| external.postgresql.port | int | `5432` |  |
| external.postgresql.postgresqlDatabase | string | `"judge"` |  |
| external.postgresql.postgresqlPassword | string | `""` |  |
| external.postgresql.postgresqlUsername | string | `"judge"` |  |
| external.redis.host | string | `"localhost"` |  |
| external.redis.password | string | `""` |  |
| external.redis.port | int | `6379` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"judge0/api"` |  |
| image.tag | string | `"1.5.0"` |  |
| livenessProbe.enable | bool | `false` | Enabling Readiness Probe |
| livenessProbe.initialDelay | int | `30` | Intial Delay to take in account |
| livenessProbe.timeout | int | `1` |  Define custom timeout |
| postgresql.enabled | bool | `true` |  |
| postgresql.image.tag | float | `9.6` |  |
| postgresql.persistence.enabled | bool | `false` |  |
| postgresql.postgresqlDatabase | string | `"judge"` |  |
| postgresql.postgresqlPassword | string | `"uaeyjbzuyq"` |  |
| postgresql.postgresqlUsername | string | `"judgemaster"` |  |
| postgresql.service.port | int | `5432` |  |
| readinessProbe.enable | bool | `true` | Enabling Readiness Probe |
| readinessProbe.initialDelay | int | `30` | Intial Delay to take in account |
| readinessProbe.interval | int | `60` | Readiness check interval |
| readinessProbe.timeout | int | `3` |  Define custom timeout |
| redis.cluster.enabled | bool | `false` |  |
| redis.enabled | bool | `true` |  |
| redis.master.persistence.enabled | bool | `false` |  |
| redis.password | string | `"a8iuw23iuizy"` |  |
| redis.redisPort | int | `6379` |  |
| service.annotations | string | `nil` |  |
| service.externalTrafficPolicy | string | `"Cluster"` |  |
| service.nodePorts.http | string | `""` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |

### FAQ
How do i pass judge0 config ?
* You can pass all the ENV that is in configuration via `values.yaml`, incase not present create and issue here or you also can create an PR for the same.

How and where to create issue?
* Incase its an configuration issue or related to Helm you can create issue [here][https://github.com/saikatharryc/helm/issues] with Title Tagged to `[Judge0]`
else related to judge0 itelf you can create [here]([here][https://github.com/judge0/api/issues])
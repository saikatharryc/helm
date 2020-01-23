# [Judge0](https://github.com/judge0/api/)

[Judge0 API](https://github.com/judge0/api/) is a free, robust and scalable open-source online code execution system.

Judge0 API can help you build wide range of applications varying from competitive programming platforms, educational and recruitment platforms, to online code editors and more.

To see Judge0 API in action, try Judge0 IDE - free and open-source code editor that uses Judge0 API for executing the user’s source code. You can also try using a dummy client, which can help you explore and test almost all the features of Judge0 API.

## Parameters

The following table lists the configurable parameters of the Judge0 chart and their default values.

| Parameter                           | Description                                                   | Default                                                  |
|-------------------------------------|---------------------------------------------------------------|----------------------------------------------------------|
| `image.registry`  |  Judge0 Image registry |   `docker.io`|
|   `image.repository`| Judge0 Image Repo name| `judge0/api` |
|   `image.tag` | Judge0 Image TAG |    `1.5.0`|
| `image.pullSecrets` | Specify docker-registry secret names as an array | `nil`|
| `service.type`	| Kubernetes Service type	|`LoadBalancer`|
| `service.port`|	Service HTTP port	|`80`|
|`service.nodePorts.http`|	Kubernetes http node port|	`""`
|`service.externalTrafficPolicy`|	Enable client source IP preservation|	`Cluster`|
|`service.loadBalancerIP`|	LoadBalancerIP for the Ghost service	|`nil`|
`service.annotations`	|Service annotations|	`nil`|
|`RAILS_MAX_THREADS` | Max Threads to use | `5`|
| `MAINTENANCE_MODE` | Turn on Maintenance Mode | `false`|
|`MAINTENANCE_MESSAGE`| Message for Maintenance, incase its active | `Judge0 API is currently in maintenance.`|
| `postgresql.enabled`| Whether or not to install Postgres (disable if using external) | `true`|
|`postgresql.postgresqlUsername` | Username for the postgres DB to create | `judgemaster`|
|`postgresql.postgresqlPassword` | Password for the postgres DB to create | `uaeyjbzuyq`|
|`postgresql.postgresqlDatabase` | Password for the postgres DB to create | `judge`|
| `redis.enabled`| Whether or not to install Redis (disable if using external) | `true`|
|`redis.password` | Password for the Redis to create | `a8iuw23iuizy`|
| `external.postgresql.host`| Host of the external postgres database|`localhost`|
 | `external.postgresql.postgresqlUsername`| User of the external postgres database|`judge`|
| `external.postgresql.postgresqlPassword`| Host of the external postgres database|`nil`|
| `external.postgresql.postgresqlDatabase`| Host of the external postgres database|`judge`|
| `external.postgresql.port`| Host of the external postgres database|`5432`|
| `external.redis.host`| Host for the external Redis instance |`localhost`|
| `external.redis.password`| Password for the external redis instance |`nil`|
| `external.redis.port`| Host of the external Redis database |`6379`|

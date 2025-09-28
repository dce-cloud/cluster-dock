# cluster-dock

基于 Docker Compose 搭建的集群服务环境

# IP地址
内部IP地址从 172.25.29.3 开始

# 服务清单

## Cluster (集群服务)
172.25.29.3 start

### Ndb Cluster (172.21.10.3~172.21.10.11)
| status | service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|---|
| phpmyadmin | 172.21.10.3 | 172.20.10.3 | latest | |
| ndb-data1 | 172.21.10.4 | 172.20.10.4 | latest | |
| ndb-data2 | 172.21.10.5 | 172.20.10.5 | latest | |
| ndb-data3 | 172.21.10.6 | 172.20.10.6 | latest | |
| ndb-data4 | 172.21.10.7 | 172.20.10.7 | latest | |
| ndb-sql1 | 172.21.10.8 | 172.20.10.8 | latest | |
| ndb-sql2 | 172.21.10.9 | 172.20.10.9 | latest | |
| ndb-management | 172.21.10.10 | 172.20.10.10 | latest | |


### RABBITMQ CLUSTER (172.21.2.3) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| rabbitmq1 | 172.21.2.3 | 172.20.2.3 | 3.12 | |
| rabbitmq2 | 172.21.2.4 | 172.20.2.4 | 3.12 | |
| rabbitmq3 | 172.21.2.5 | 172.20.2.5 | 3.12 | |

### KAFKA KRAFT CLUSTER (172.21.2.13) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| krc-kafka-ui | 172.21.2.13 | 172.20.2.210 | 3.6 | |
| krc-kafka1 | 172.21.2.13 | 172.20.2.211 | 3.6 | |
| krc-kafka2 | 172.21.2.13 | 172.20.2.212 | 3.6 | |
| krc-kafka3 | 172.21.2.13 | 172.20.2.213 | 3.6 | |
| krc-kafka4 | 172.21.2.13 | 172.20.2.214 | 3.6 | |
| krc-kafka5 | 172.21.2.13 | 172.20.2.215 | 3.6 | |
| krc-kafka6 | 172.21.2.13 | 172.20.2.216 | 3.6 | |

### KAFKA CLUSTER (172.21.2.30) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| kc-kafka-ui | 172.21.2.220 | 172.20.2.220 | latest | |
| kc-zoonavagitor | 172.21.2.221 | 172.20.2.221 | | |
| kc-zoo | 172.21.2.222 | 172.20.2.222 | latest | |
| kc-kafka1 | 172.21.2.223 | 172.20.2.223 | latest | |
| kc-kafka2 | 172.21.2.224 | 172.20.2.224 | latest | |
| kc-kafka3 | 172.21.2.225 | 172.20.2.225 | latest | |
| kc-kafka4 | 172.21.2.226 | 172.20.2.226 | latest | |
| kc-kafka5 | 172.21.2.227 | 172.20.2.227 | latest | |
| kc-kafka6 | 172.21.2.228 | 172.20.2.228 | latest | |

### ROCKETMQ CLUSTER (172.21.2.50) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| rocketmq-dashboard | 172.21.2.11 | 172.20.2.11 | latest | |
| rocketmq-c-namesrv1 | 172.21.2.11 | 172.20.2.3 | latest | |
| rocketmq-c-namesrv2 | 172.21.2.11 | 172.20.2.4 | latest | |
| rocketmq-c-namesrv3 | 172.21.2.11 | 172.20.2.5 | latest | |
| rocketmq-c-proxy1 | 172.21.2.11 | 172.20.3.6 | latest | |
| rocketmq-c-proxy2 | 172.21.2.11 | 172.20.3.7 | latest | |
| rocketmq-c-proxy3 | 172.21.2.11 | 172.20.3.8 | latest | |
| rocketmq-c-controller1 | 172.21.2.11 | 172.20.3.9 | latest | |
| rocketmq-c-controller2 | 172.21.2.11 | 172.20.3.10 | latest | |
| rocketmq-c-controller3 | 172.21.2.11 | 172.20.3.11 | latest | |
| rocketmq-c-broker1 | 172.21.2.11 | 172.20.3.12 | latest | |
| rocketmq-c-broker2 | 172.21.2.11 | 172.20.3.13 | latest | |
| rocketmq-c-broker3 | 172.21.3.14 | 172.20.3.14 | latest | |
| rocketmq-c-broker4 | 172.21.3.15 | 172.20.3.15 | latest | |
| rocketmq-c-broker5 | 172.21.3.16 | 172.20.3.16 | latest | |
| rocketmq-c-broker6 | 172.21.3.17 | 172.20.3.17 | latest | |

### Pulsar Cluster (172.21.2.70) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| pulsar-manager | 172.21.2.82 | 172.20.2.82 | 0.4.0 |
| pulsar-zookeeper | 172.21.2.81 | 172.20.2.81 | latest |
| pulsar-init | 172.21.2.80 | 172.20.2.80 | latest |
| pulsar-bookie1 | 172.21.2.83 | 172.20.2.83 | latest |
| pulsar-bookie2 | 172.21.2.84 | 172.20.2.84 | latest |
| pulsar-bookie3 | 172.21.2.85 | 172.20.2.85 | latest |
| pulsar-broker1 | 172.21.2.86 | 172.20.2.86 | latest |
| pulsar-broker2 | 172.21.2.87 | 172.20.2.87 | latest |
| pulsar-broker3 | 172.21.2.88 | 172.20.2.88 | latest |

### NSQ CLUSTER (172.21.2.90) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| nsqadmin | 172.21.2.110 | 172.20.2.110 | latest | |
| nsqlookupd1 | 172.21.2.111 | 172.20.2.111 | latest | |
| nsqlookupd2 | 172.21.2.112 | 172.20.2.112 | latest | |
| nsqlookupd3 | 172.21.2.113 | 172.20.2.113 | latest | |
| nsqd1 | 172.21.2.101 | 172.20.2.101 | latest | |
| nsqd2 | 172.21.2.101 | 172.20.2.101 | latest | |
| nsqd3 | 172.21.2.101 | 172.20.2.101 | latest | |

### NATS CLUSTER (172.21.2.100) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| nats-box | 172.21.2.240 | 172.20.2.240 | latest | |
| nats1 | 172.21.2.241 | 172.20.2.241 | latest | |
| nats2 | 172.21.2.242 | 172.20.2.242 | latest | |
| nats3 | 172.21.2.243 | 172.20.2.243 | latest | |

### ETCD CLUSTER (172.21.2.110) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| ec-etcd-ui | 172.21.2.170 | 172.20.2.170 | | |
| ec-etcd1 | 172.21.2.171 | 172.20.2.171 | v3.5.2 | |
| ec-etcd2 | 172.21.2.172 | 172.20.2.172 | v3.5.2 | |
| ec-etcd3 | 172.21.2.173 | 172.20.2.173 | v3.5.2 | |

### ZOOKEEPER CLUSTER (172.21.2.120) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| zc-zoonavagitor | 172.21.2.190 | 172.20.2.190 | | |
| zookeeper1 | 172.21.2.191 | 172.20.2.191 | latest | |
| zookeeper2 | 172.21.2.192 | 172.20.2.192 | latest | |
| zookeeper3 | 172.21.2.193 | 172.20.2.193 | latest | |

### DTM CLUSTER (172.21.2.130) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| dtm-mysql | 172.21.3.80 | 172.20.3.80 | latest |
| dtm-redis | 172.21.3.81 | 172.20.3.81 | latest |
| dtm1 | 172.21.3.82 | 172.20.3.82 | latest |
| dtm2 | 172.21.3.83 | 172.20.3.83 | latest |
| dtm3 | 172.21.3.84 | 172.20.3.84 | latest |

### MEMCACHED CLUSTER (172.21.2.140) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| memcached1 | 172.21.3.180 | 172.20.3.180 | latest | |
| memcached2 | 172.21.3.181 | 172.20.3.181 | latest | |
| memcached3 | 172.21.3.182 | 172.20.3.182 | latest | |
| haproxy1 | 172.21.3.183 | 172.20.3.183 | latest | |

### MINIO CLUSTER (172.21.2.150) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| nginx | 172.21.3.140 | 172.20.3.140 | latest | |
| minio1 | 172.21.3.141 | 172.20.3.141 | latest | |
| minio2 | 172.21.3.142 | 172.20.3.142 | latest | |
| minio3 | 172.21.3.143 | 172.20.3.143 | latest | |

### REDIS MSR (172.21.2.160) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| redis_1 | 172.21.3.180 | 172.20.3.180 | latest | |
| redis_2 | 172.21.3.181 | 172.20.3.181 | latest | |
| redis_3 | 172.21.3.182 | 172.20.3.182 | latest | |
| redis_4 | 172.21.3.183 | 172.20.3.183 | latest | |
| sentinel1 | 172.21.3.184 | 172.20.3.184 | latest | |
| sentinel2 | 172.21.3.185 | 172.20.3.185 | latest | |
| sentinel3 | 172.21.3.186 | 172.20.3.186 | latest | |

### REDIS CLUSTER (172.21.2.170) [完成]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| redis-box | 172.21.3.190 | 172.20.3.190 | latest | |
| redis1 | 172.21.3.191 | 172.20.3.191 | latest | |
| redis2 | 172.21.3.192 | 172.20.3.192 | latest | |
| redis3 | 172.21.3.193 | 172.20.3.193 | latest | |
| redis4 | 172.21.3.194 | 172.20.3.194 | latest | |
| redis5 | 172.21.3.195 | 172.20.3.195 | latest | |
| redis6 | 172.21.3.196 | 172.20.3.196 | latest | |
| redis7 | 172.21.3.197 | 172.20.3.197 | latest | |
| redis8 | 172.21.3.198 | 172.20.3.198 | latest | |
| redis9 | 172.21.3.199 | 172.20.3.199 | latest | |

### NACOS CLUSTER (172.21.2.190) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| nacos1 | 172.21.3.211 | 172.20.3.211 | latest | |
| nacos2 | 172.21.3.211 | 172.20.3.211 | latest | |
| nacos3 | 172.21.3.211 | 172.20.3.211 | latest | |

### ELASTIC CLUSTER (172.21.2.200) [待定]
| service | backend ip | frontend ip | version | 备注 |
|---|---|---|---|---|
| es-setup | 172.21.2.200 | 172.20.2.200 | latest |
| kibana | 172.21.2.201 | 172.20.2.201 | latest |
| es01 | 172.21.2.202 | 172.20.2.202 | latest |
| es02 | 172.21.2.203 | 172.20.2.203 | latest |
| es03 | 172.21.2.204 | 172.20.2.204 | latest |


# 使用到的镜像
- 默认使用docker.io 镜像
- 若想使用自定义仓库镜像，需要定义 `DOCKER_REGISTRY_URL` 变量

```json
[
    "traefik:v3.4",
]
```

![](docs/images/logo_radondb-mysql.png) <br>

English | [中文](README_zh.md) 

# What is RadonDB MySQL

[RadonDB MySQL](https://github.com/radondb/radondb-mysql-kubernetes) is an open-source, cloud-native, highly availability cluster solutions based on [MySQL](https://MySQL.org). With the Raft protocol，RadonDB MySQL provides faster failover performance without losing any transactions.

## RadonDB MySQL Kubernetes

RadonDB MySQL Kubernetes supports deployment and management of RaodnDB MySQL clusters on [Kubernetes](https://kubernetes.io) or [KubeShpere](https://kubesphere.com.cn) and automates tasks related to operating a RadonDB MySQL cluster.

## Architecture

- Decentralized leader automatic election through Raft protocol.
- Synchronizing data based on GTID mode through Semi-Sync.
- Supporting high-availability through [Xenon](https://github.com/radondb/xenon.git).

![](docs/images/radondb-mysql_Architecture_1.png)

## Features

- High availability MySQL database
    - Non-centralized automatic leader selection
    - Leader-follower switching in second-level
    - Strongly consistent data for cluster switching
- Cluster management
- Monitoring and alerting
- Logs
- Account management

## Quick Start

- [Deploy RadonDB MySQL on Kubernetes](docs/Kubernetes/deploy_radondb-mysql_on_kubernetes.md)
- [Deploy RadonDB MySQL on appstore of KubeSphere](docs/KubeSphere/deploy_radondb-mysql_on_kubesphere.md)

## Roadmap

| Release | Features  | Mode |
|------|--------|--------|
| 1.0 | High availability <br>  Non-centralized automatic leader election <br>  Second-level switching <br>  Strongly consistent data <br> Cluster management <br> Monitoring and alerting <br> Logs <br> Account management | Helm |
| 2.0 | Node management <br> Automatic expansion and shrinkage capacity <br> Upgrade <br> Backups and Restorations <br> Automatic failover <br> Automatic rebuild node <br> Automatic restart service（all or signal node）<br> Account management（API）<br> Migrating Data online | Operator |
| 3.0 | Automatic O&M <br> Multiple node roles <br> Disaster Recovery <br> SSL transmission encryption  | Operator |

## Who are using RadonDB MySQL

![](docs/images/users.png)

## License

RadonDB MySQL is released under the Apache 2.0, see [LICENSE](./LICENSE).

## Discussion and Community

- Forum

    The RadonDB MySQL topic is in [Kubesphere Community](https://kubesphere.com.cn/forum/t/radondb).

- WeChat group
    
    To enter the wechat group of radondb community, please add administrator wechat.
    
    ![](docs/images/wechat_admin.jpg)

Please submit any RadonDB MySQL bugs, issues, and feature requests to RadonDB MySQL GitHub Issue.

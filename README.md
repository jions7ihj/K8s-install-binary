# k8s-install-binary

- 本文主要介绍如何使用官方提供的二进制包部署K8S（V1.13.3）集群。同时具有以下几大特性

  - TLS双向认证
  - RBAC授权
  - Flannel网络
  - ETCD高可用集群
  - Kube-proxy 启用ipvs

- k8s架构图

  ![kubernetes](https://github.com/hikubernetes/k8s-install-binary/blob/master/images/k8s%E6%9E%B6%E6%9E%84.png)



* 集群分布架构图

  | Role   | Hostname | IP            |
  | ------ | -------- | ------------- |
  | master | master   | 192.168.175.3 |
  | worker | node01   | 192.168.175.4 |
  | worker | node02   | 192.168.175.5 |

* 
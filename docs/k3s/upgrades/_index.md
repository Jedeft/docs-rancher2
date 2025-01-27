---
title: "升级介绍"
description: 本节介绍如何升级 K3s 集群。
keywords:
  - k3s中文文档
  - k3s 中文文档
  - k3s中文
  - k3s 中文
  - k3s
  - k3s教程
  - k3s中国
  - rancher
  - k3s 中文教程
  - 升级介绍
---

本节介绍如何升级 K3s 集群。

[基础升级](/docs/k3s/upgrades/basic/_index)描述了手动升级集群的几种技术。它也可以作为通过第三方基础设施即代码工具（如[Terraform](https://www.terraform.io/)）进行升级的基础。

[自动升级](/docs/k3s/upgrades/automated/_index)描述了如何使用 Rancher 的[system-upgrade-controller](https://github.com/rancher/system-upgrade-controller)执行 Kubernetes 原生的自动升级。

> 如果 Traefik 没有被禁用，K3s 1.20 及以前的版本会安装 Traefik v1，而 K3s 1.21 及以后的版本会安装 Traefik v2（如果还没有 v1）。 要升级 Traefik，请参考[Traefik 文档](https://doc.traefik.io/traefik/migration/v1-to-v2/)，并使用[迁移工具](https://github.com/traefik/traefik-migration-tool)从旧的 Traefik v1 迁移到 Traefik v2。
> 
> 在 K3s v1.19.1 中，实验性的嵌入式 Dqlite 数据存储被废弃了。请注意，不支持从实验性 Dqlite 到实验性嵌入式 etcd 的升级。如果你尝试升级，它将不会成功，数据将丢失。

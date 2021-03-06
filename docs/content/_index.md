---
title: "自动化部署 ELK"
weight: 100
draft: false
---

# 自动化部署
# ElasticSearch + Logstash + Kibana

本项目使用 [Ansible](https://www.ansible.com/) 作为自动化部署工具，实现“自动化部署” [ELK](https://www.elastic.co/)（Elastic Search + Logstash + Kibana）生产集群。

## 项目特性

* 集成 [Consul](https://www.consul.io/) 服务发现注册。
* 集成 [Monit](https://mmonit.com/monit/) 监控，附带配套的 Kibana 看板。
* 集成 [Curator](https://www.elastic.co/guide/en/elasticsearch/client/curator/current/index.html) 对 indices 进行日常定时维护。
* **ES 可以划分多种角色，实现冷热数据等架构规划。**
* **包括升级脚本，可实现集群平滑版本升级。**
* **支持离线部署方式，生产环境无需访问外网。**
* 修改过的服务器配置文件，会下载到本地 install_report 目录下，方便核对结果。

## 适用平台
#### 本项目基于 ansible 2.7.5 测试通过以下版本和环境。

| Elastic version | Ubuntu Server 16.04 | CentOS 7 |
| --------------- | ------------------- | -------- |
| 6.5.x           | Yes                 | Yes      |
| 6.4.x           | Yes                 | Yes      |

## 目录
{{% children sort="weight" depth="1" %}}

## 关于我

喜欢折腾 Linux 运维的汉语言文学师范专科毕业生。

现为 [新致云](https://cloud.newtouch.com/) 架构师。

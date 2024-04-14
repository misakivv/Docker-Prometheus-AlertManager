# Docker-Prometheus-AlertManager

如何使用Docker部署Prometheus、Grafana与Alertmanager，并实现基于邮件的告警功能

## 一、涉及主机

### 1、硬件准备（虚拟机）

|    主机名     |     IP地址     |
| :-----------: | :------------: |
|    server     | 192.168.112.40 |
| node-exporter | 192.168.112.50 |

## 二、步骤

一、环境准备

​	1、硬件准备（虚拟机）
​	2、关闭防火墙，selinux
​	3、所有主机安装docker

二、配置Prometheus

​	1、docker启动Prometheus

三、添加监控节点

​	1、docker启动node-exporter

四、Prometheus配置node-exporter

​	1、修改prometheus.yml配置文件

五、配置Alertmanager

​	1、docker启动Alertmanager

六、Alertmanager配置邮件告警

七、配置Alertmanager告警规则

​	1、创建报警规则文件`node-up.rules`
​	2、然后修改 `prometheus.yml` 配置文件，添加 rules 规则文件。

八、触发报警发送Email

​	1、停止服务测试

九、Alertmanager配置自定义邮件模板

​	1、创建一个模板文件

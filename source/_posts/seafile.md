---
title: seafile
date: 2018-02-07 15:24:29
tags:
---

### sealfile简介

Seafile 是一个开源的文件云存储平台，解决文件集中存储、同步、多平台访问的问题，注重安全和性能。
Seafile 通过“资料库”来分类管理文件，每个资料库可单独同步，用户可加密资料库， 且密码不会保存在服务器端，所以即使是服务器管理员也无权访问你的文件。
Seafile 允许用户创建“群组”，在群组内共享和同步文件，方便了团队协同工作。

### 安装

准备：一台服务器，我用的是阿里云服务器ECS
可以用[官方](https://manual-cn-origin.seafile.com/)的[快速安装方法](https://github.com/haiwen/seafile-server-installer-cn)进行安装

### 配置

阿里云服务器的安全组规则中打开下面两个端口：

1. seafile fileserver 负责为 Seahub 处理文件的上传和下载
- 默认端口：8082
- 配置文件：seafile/conf/seafile.conf
2. seahub 是 Seafile 服务器的 Web 端
- 默认端口：8000
- 配置文件：seafile/conf/ccnet.conf

详情请见官方文档中包含[端口说明](https://manual-cn.seafile.com/deploy_windows/ports_used_by_seafile_windows_server.html)

### 登录
网页登录：ip:8000 or 域名:8000
客户端登录：[下载地址](https://www.seafile.com/download/)
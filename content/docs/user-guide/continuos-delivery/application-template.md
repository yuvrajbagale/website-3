﻿+++
title = "应用模板"
description = ""
weight = 1
+++

# 应用模板
  
  应用模板是将同类型应用的代码库结构整理成模板，用于创建应用时能引用相应模板快速创建初始代码库。 每种应用模板至少都包括CI文件以及Chart目录文件。 平台提供默认的常用模板，用户可以根据实际情况自定义符合更多需求的应用模板。

  - **菜单层次**：组织层
  - **菜单路径**：持续交付 > 应用模板
  - **默认角色**：平台管理员、项目创建者

### 新建应用模板

  输入应用模板编码，名称，描述，创建默认最简模板。您也可以通过复制于现有模板，以便节省部分共同操作，提升效率。

   1. 点击`创建应用模板`按钮；

   1. 输入应用相关信息，点击`创建`按钮；

   1. 本地克隆应用模板对应的代码库。
      一个正确的模板中应该包含:
spring-boot项目+gitlab-ci.yml文件+dockerfile文件+charts模块

      >spring-boot项目: 模板项目

      >gitlab-ci.yml文件: 定义gitlab ci的阶段

      >dockerfile文件: 用于应用部署时生成镜像

      >charts模块: 用于创建应用时生成创建k8s对象 

如:deployment job service ingress,部署时配置信息里的key-value值会被应用到对应的k8s对象中用于部署。

### 查看应用详情

  在详情界面根据应用模板名称、应用模板编码、应用模板描述、应用模板地址、应用模板来源来查看应用详情。

列表字段

 - 应用模板名称：应用模板的自定义名称。
 - 应用模板编码：应用模板的自定义编码。
 - 应用模板描述：应用模板的自定义描述。
 - 应用模板地址：应用模板的git仓库地址。
 - 应用模板来源：应用模板的来源。

### 修改模板信息
点击`修改模板`→ ![修改环境按钮](/docs/user-guide/continuos-delivery/image/修改环境按钮.png)按钮 ，进行应用模板名称和描述的修改。

### 删除模板信息
点击`删除模板`→ ![删除网络按钮](/docs/user-guide/continuos-delivery/image/删除网络按钮.png) 按钮，进行模板的删除。
<blockquote class="warning">
         若删除模板，该条数据将被永久删除，不可恢复!
      </blockquote>
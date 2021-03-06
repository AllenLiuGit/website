﻿+++
title = "环境流水线"
description = ""
weight = 1
+++

# 环境流水线

环境是指一个应用可以被部署的地方。常见环境有开发测试环境、预生产环境、生产环境等。Choerodon 自动为您的项目生成一条环境流水线，用户可以根据需要调整顺序环境的顺序，通过环境流水线，用户可以清晰地定义和查看应用部署的顺序。

  
  - **菜单层次**：项目层
  - **菜单路径**：持续交付 > 部署管理 > 环境流水线
  - **默认角色**：项目所有者、项目成员、部署管理员
    <blockquote class="note">
         项目所有者和项目成员对环境流水线只有查看界面的权限，不可进行编辑修改。
      </blockquote>

### 创建环境

   1. 点击 `创建` 按钮；

   1. 输入 “环境编码” 、 “环境名称” 以及 “环境描述” ，点击 `创建` 按钮；
<blockquote class="note">
          新环境默认新增在环境流水线的最后一个节点。
      </blockquote>

 1. 创建的环境可以任意拖拽，调换环境之间的位置。

### 查看环境流水线详情

 1. 进入持续交付后，点击 `环境流水线` 页签；

 1. 查看应用环境的运行情况。

>- 在环境卡片中，点击`复制指令`→ ![复制指令按钮](/docs/user-guide/Assembly line/image/复制指令按钮.png) ，复制代码至Kubernetes运行，与平台建立链接。
>- 在环境卡片中，点击`修改环境`→ ![修改环境按钮](/docs/user-guide/Assembly line/image/修改环境按钮.png) ，修改环境名称及描述。
>- 在环境卡片中，点击`禁用环境`→ ![停用按钮](/docs/user-guide/Assembly line/image/停用按钮.png) ，当点击确认后，该环境将被禁用。

### 环境停用区 

可在环境停用区查看已被停用的环境，点击卡片右上角`启用按钮` → ![启用按钮](/docs/user-guide/Assembly line/image/启用按钮.png) 重新启用。
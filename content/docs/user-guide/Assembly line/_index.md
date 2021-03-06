﻿+++
title = "开发流水线"
description = ""
weight = 2
+++

<h2 id="1">介绍</h2>
开发流水线中描述了集成 Gitlab 作为代码托管的仓库，以及采用 Gitflow 分支模型进行一个应用的管理。可以查看应用的所有版本信息、应用编码、应用名称及版本创建时间，并描述了应用的持续集成流水线信息。

<h2 id="2">功能</h2>

 - [**应用模板**](../assembly-line/application-template) 是将同类型应用的代码库结构整理成模板，用于创建应用时能引用相应模板快速创建初始代码库。

 - [**应用管理**](../assembly-line/application-management) 一个系统可以被解耦成很多应用，每一个应用都可以独立部署，每一个应用仅关注于完成一部分任务，每部分任务代表一个小的业务模块，因此各应用之间关系是松耦合的。另外，每创建一个应用，系统会自动在gitlab创建好对应的代码库。

 - [**分支管理**](../assembly-line/branch-management) 采用的 Gitflow 工作流模式，有Master和Develop两个默认分支。在持续交付过程中对 Feature、Release、Hotfix 等分支进行管理。结束分支可自动触发分支合并和持续集成，可在流水线查看代码集成情况。

 - [**持续集成**](../assembly-line/assembly-line) 是 Gitlab 自带的持续集成引擎，免去了第三方 CI 服务器只能定时检测 git 仓库带来的延迟和对 Git Server 造成的性能压力。能够解决的问题有小步伐的产品迭代，高频率的版本发布，随时随地的系统集成等，达到效率极大增加的作用。

 - [**应用版本**](../assembly-line/service-version) 由于 Choerodon 采用 Gitflow 的方式管理分支，所以对于版本的控制也是根据 Feature、Release、Hotfix 等分支上进行的。
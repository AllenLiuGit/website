﻿+++
title = "敏捷管理"
description = ""
weight = 2
draft = true
+++

# 敏捷管理

<h2 id="1">介绍</h2>

   敏捷管理服务简单说就是灵活+快速，既满足产品开发过程中需求的动态变化，又能通过短迭代管理监控项目的实时效果。敏捷管理方法充分考虑到了可能出现的不确定性因素，同时具有鲜明的创造性。它的结构是围绕着学习过程建立的，这样一来，团队既可以评估已经取得的成果，同样重要的是，也可以评估取得这些成果的方法。这种架构能够为团队提供更加高效的工作方式，帮助他们更好地自我组织，提高工作速度，改进工作质量。

<h2 id="2">功能</h2>

 - 集成Gitlab，实现 [**用户故事**](../scrum/user-story)、[**任务**](../scrum/task)、[**漏洞**](../scrum/bug)、[**冲刺**](../scrum/sprint) 等卡片的创建、更新、删除、查询。
 - 项目创建后默认创建空白看板，可根据项目的需要选择合适的看板模板，用户也可自定义绘制看板。支持 [**看板**](../scrum/board) 内卡片的拖动以及状态的实时更新。
 - 根据项目的需求可创建冲刺，用户故事来源于故事地图里的发布计划。 用户可同时开启一个冲刺，对应的卡片会同步到看板中，实现冲刺与看板一对一的关系。
 - 关闭冲刺后将当前看板保存为历史看板，以及将未完成的用户故事退回到故事地图中，同时将其下的任务、缺陷删除。
 - 实现用户故事、任务、缺陷的全局查询，以及快捷方式创建、修改、删除。
 - 集成文件服务、minio等对项目附件集中存储，提供附件的上传、下载、删除功能。
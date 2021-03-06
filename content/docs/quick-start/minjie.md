﻿+++
title = "使用敏捷管理工具"
description = ""
weight = 5
draft = true
+++

# 使用敏捷管理工具
## 概述
Choerodon认为软件交付过程的本质是用户价值的实现，而用户价值的实现是通过用户价值流动来体现的，Choerodon提供了一套工具来帮助用户通过敏捷的方式来管理用户价值的流动，使整个软件开发流程管理化规范化。

敏捷管理是以用户需求演变为中心，通过迭代方式来进行的软件开发。Choerodon敏捷管理的核心是需求，计划和执行。即通过故事地图、用户故事来管理用户故事和发布计划，通过迭代来管理冲刺，最后通过看板来可视化冲刺的执行。

## 目标

本页面主要介绍choerodon的敏捷管理，从创建用户故事地图、冲刺管理、敏捷看板等功能介绍使用方法，使用户阅读整个流程后，能够熟知整个操作流程。

<h2 id="1">创建用户故事地图</h2>

故事地图已经成为敏捷管理在需求规划中的一个重要的方法。Choerodon的故事地图可以将你的用户故事（user stories）像地图一样展现出来，而不是传统的简单列表形式。

 **1.创建角色**
 

 - 使用项目所有者或者源代码管理员的角色登录Choerodon系统，选择项目`猪齿鱼研发`。
 
 - 选择敏捷管理模块，点击`故事地图`，点击`创建角色`按钮，将鼠标移动至角色列，此时鼠标变为十字形，点击即可创建一个角色；
 
 - 再次点击`创建项目`，选中刚才创建的角色卡，输入角色名称，点击`保存`，可修改角色名称。

      ![](/docs/quick-start/image/story-map.png)
  

 **2.创建活动**

 - 点击`创建活动`按钮，将鼠标移动至活动列，此时鼠标变为十字形，点击即可创建一个活动；
 
 - 再次点击`创建活动`，选中刚才创建的活动卡，输入活动名称，点击`保存`，可修改活动名称。

**3.创建任务**

 - 点击`创建任务`按钮，将鼠标移动至任务列，此时鼠标变为十字形，点击即可创建一个活动；
 
 - 再次点击`创建任务`，选中刚才创建的任务卡，输入任务名称，点击`保存`，可修改任务名称。

**4.创建故事**


 - 点击`发布计划`按钮，将鼠标移动至发布计划列表下，点击`创建故事`，即可创建一个故事；选中刚才创建的故事卡，输入故事名称，点击`保存`，可修改故事名称。
   <blockquote class="note">
     当故事较多时，可点击添加故事列表进行添加。
    </blockquote>
2. 点击‘导出为图片’按钮可导出当前故事地图的图片。
   <blockquote class="note">
    故事地图页面的滑动轴可调整压面大小。
    </blockquote>

<h2 id="1">迭代冲刺</h2>

用迭代来管理冲刺，每一个迭代对应一次冲刺，也可以简单理解为每一次冲刺就是一个迭代周期。在固定的时间内，要完成需求分析、设计、实现、测试等一系列活动，在迭代周期完成的时候提供一个可工作的产品。每一次迭代完成的可能是一个或几个完整的用户故事，也可能是一个用户故事中的若干用户任务。

**1.创建冲刺**

 - 选择敏捷管理模块，点击`冲刺`，进入冲刺管理页面，点击`创建冲刺`，会弹出一个侧边框，填写相关信息；
 
　　a 选择发布计划：选择刚才创建的发布计划
	
　　b 冲刺名称：填写冲刺名称

　　c 冲刺目标：填写冲刺目标

　　d 时长：选择冲刺时间
	
　　e 预计开始时间：选择预计开始时间
	
　　f 预计结束时间：选择预计结束时间

 - 信息填写完成以后，点击`创建`即可。

**2.导入用户故事**

 - 回到冲刺管理界面，可以查看刚才创建的冲刺，点击`冲刺名称`，进入冲刺详情界面。
 
 - 点击`导入用户故事`，选择`导入的冲刺`和`导入的用户故事`，点击`确定`可导入之前创建的故事地图。故事地图会同步生成的ID显示在界面上。
 
    <blockquote class="note">
   冲刺管理界面中的待办事项可向冲刺里拖拽状态为product backlog的用户故事、任务、缺陷，拖拽后的issue会关联到该冲刺中。
    </blockquote>
	
 - 冲刺里的issue都添加好之后，用户可点击`开始冲刺`按钮开启冲刺。
 
    <blockquote class="note">
    冲刺开启后，issue的信息会同步到看板中，之后用户可在看板中操作。
    </blockquote>

 
 - 点击冲刺后可跳转到冲刺详情，该详情页面记录当前冲刺的用户故事、任务、缺陷的完成情况，以及故事点、工作量、进度等信息。冲刺燃尽图、时间前置图、累计流图是冲刺的三个统计图表。
 
 - 冲刺下的用户故事、任务、缺陷详情页面可修改该issue的具体信息，包括优先级、负责人、工作预估、工作日志、描述等，用户之间还可在评论模板下对该issue展开讨论。

<h2 id="1">看板管理</h2>

我们都知道在软件开发过程中，短板或者瓶颈会直接的影响整个开发进程。看板方法是用于高效管理软件开发流程的新技术。Choerodon看板是Choerodon敏捷管理中执行部分，它的核心作用是可视化整个迭代的计划执行，并且暴露开发执行过程中的短板或者瓶颈。

**1.选择模板**

 - 选择敏捷管理模块，点击`看板`，进入看板页面；
 
 - 点击`选择模板`，选中相应的模板后，点击`确定`；您也可以自定义一个模板。
   <blockquote class="warning">
      非sprint  backlog列无卡片时可选择。
    </blockquote>
 - 点击看板右上方的编辑按钮可进入到看板绘制页面，该页面可增删改看板列、泳道，设置在制品、起始列、终止列等，绘制完毕后点保存按钮即可。
 
 **2.创建修改故事卡片**
 
 - 看板中可创建卡片，创建后的卡片会同步到对应的冲刺与发布计划中。点击`创建卡片`键，如下图，填写相关信息，点击`保存`即可。
 
      ![](/docs/quick-start/image/kanban.png)
	  
 - 点击issue卡片，可查看issue详情，点击`编辑`，可对标题、负责人、需求类型等信息进行修改；
 
 - 根据项目进度，可调整故事卡片的位置，拖拽故事卡片至相应的位置即可；
    <blockquote class="note">
     issue下有子卡的，可将子卡拖拽到看板中，对应的子卡数量相应减少。
    </blockquote>
 
 - 当此次迭代（冲刺）完成后，可到冲刺管理页面关闭冲刺，冲刺关闭后将生成历史看板，完整保存关闭冲刺时的看板页面，进入到历史看板中只可查看相关issue的信息，不可增删改等。

<h2 id="1">Issue管理</h2>

 1. 展示的是当前项目的所有用户故事、任务、缺陷，点击issue可查看、修改详情。
 2. 页面可创建卡片，创建后会同步到故事地图的未规划区中。

<h2 id="1">用户故事</h2>

 - 选择敏捷管理模块，点击`用户故事`，进入故事管理页面；
 
 - 点击`创建故事`，填写填写相关信息；
	  
 - 点击`保存`，即可创建一个用户故事；


<h2 id="1">任务管理</h2>

 - 选择敏捷管理模块，点击`任务`，进入任务管理页面；
 
 - 点击任务右侧详情，可查看修改详情。
	  
      ![](/docs/quick-start/image/renwu.png)


<h2 id="1">缺陷管理</h2>

 - 选择敏捷管理模块，点击`漏洞`，进入漏洞管理页面；
	  
 - 点击缺陷右侧详情，可查看修改缺陷。
 

<h2 id="1">总结</h2>

敏捷开发作为一种面临迅速变化的需求，快速开发出高质量软件产品的新方法，自问世以来，对软件开发起着积极而又重要的影响，颇受业内人士推崇。由于软件在规模、复杂度、功能上的极大扩展和提高，以及在需求和技术不断变化的过程中实现软件自身开发的需求，敏捷开发正逐渐成为软件开发的新模式。因此，我们应当更好的利用这种方法，适应快速的需求变化，达到完善需求分析，改进开发过程，提高软件项目管理水平的目的，扩展它的应用领域。
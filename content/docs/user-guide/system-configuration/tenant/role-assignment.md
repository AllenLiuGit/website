﻿+++
title = "组织角色分配"
weight = 3
+++

# 组织角色分配

组织角色分配时，可以给一到多个成员分配一到多个角色。角色是权限的集合，给成员分配角色即给成员赋予权限。权限与角色都具有层级性，且角色权限的层级必须与角色层级相同。角色分配具有层级性，角色分配中被分配的角色层级必须与角色分配的层级相同。即，在某一层级的角色分配中，只能给用户分配对应的层级的角色，只能给角色分配对应层级的权限。例如，在组织层角色分配中，只能给用户分配组织层角色，分配后用户具有使用组织层权限。

![](/docs/user-guide/system-configuration/tenant/image/member_role3.png)

  - **菜单层次**：组织层
  - **菜单路径**：组织管理 > 组织角色分配
  - **默认角色**：组织管理员

<h2 id="1">成员角色列表</h2>

列表查看方式：

- 按成员查看：列表项为成员信息和该成员的所有角色。可以直接对成员的角色进行更改操作。
- 按角色查看：列表项为角色。展开角色后，展示信息为角色下的成员信息。可以直接对角色下的成员进行更改操作。

列表字段-按成员查看时：

- 成员：若成员为用户，则为用户的登录名；若成员为微服务，则为微服务名称。
- 名称：若成员为用户，则为用户的用户名。
- 角色：角色名称。可以为一到多个。每一个角色都可以在列表中直接删除，或点击编辑，进入编辑成员角色的界面更改成员的角色。
- 成员类型：成员类型可以为用户、微服务。

列表字段-按角色查看时：

- 角色/成员：列表的列表项为角色名称。列表项展开后的子列表为角色下的成员,若成员为用户，则为用户的登录名；若成员为微服务，则为微服务名称。
- 名称：若子列表中的成员为用户，则名称为用户名。

<h2 id="2">成员角色查询</h2>

可查询字段:

- 成员：若成员为用户，按用户的登录名查找；若成员为微服务，按微服务名称查找。
- 名称：若成员为用户，按用户的用户名查找。
- 成员类型：分用户和微服务两种。
- 角色：按角色名称查找。
   
<h2 id="3">添加成员角色</h2>

1.点击`添加`→![添加](/docs/user-guide/system-configuration/platform/image/添加.png) 添加成员角色；

2.输入`成员`、`选择一个角色`；

<blockquote class="note">
        添加新的成员角色之间的关联：如果成员已经被分配过角色，则将本次操作新增的与该成员有关的成员角色关联合并到已有关联列表，即已有的不变，新增的增加。
      </blockquote>

3.点击`添加`完成添加成员角色。

#### 层级规则：

组织层角色分配的添加成员角色为，在一个组织中，给成员添加组织层角色。例如，在运营组织这个组织中，给登录名为123的用户添加组织管理员的角色，且组织管理员这个角色满足角色层级为组织层的条件。

#### 对应规则：

成员输入一个到多个。如果成员为用户，则输入用户的登录名，若成员为应用，则输入应用名称。

角色选择一到多个。根据角色名称进行选择。可以对角色名称进行过滤。

<h2 id="4">移除成员角色</h2>

点击`移除`→![移除](/docs/user-guide/system-configuration/platform/image/移除.png) 移除成员角色；

可以进行批量删除，即可以一次性删除与某个成员或角色有关的所有成员角色关联。

- 按成员查看时：勾选一或多个成员，点击移除，批量删除所选成员和成员下所有角色的关联关系。
- 按角色查看时：勾选一或多个角色，点击移除，批量删除所选角色和角色下所有成员的关联关系。

<h2 id="5">删除成员角色</h2>

- 按成员查看时，点击`删除`→![删除按钮](/docs/user-guide/system-configuration/platform/image/删除按钮.png)，可直接删除与该成员有关联的角色，即删除了一个成员角色关联。
- 按角色查看时，点击`删除`→![删除按钮](/docs/user-guide/system-configuration/platform/image/删除按钮.png)，可直接删除与该角色有关联的成员，即删除了一个成员角色关联。
- 按成员或角色查看时，点击编辑图标，进入编辑成员的角色界面，点击`删除`→![删除按钮](/docs/user-guide/system-configuration/platform/image/删除按钮.png)，可删除与成员有关联的一个角色。

<h2 id="6">修改成员的角色</h2>

点击`编辑`→![修改](/docs/user-guide/system-configuration/platform/image/修改.png)，进入编辑一个成员的所有角色界面，可编辑该成员的角色关联。即可以删除角色，更改已有角色，添加其他角色。只有上一个角色已选时才可以继续添加其他角色。
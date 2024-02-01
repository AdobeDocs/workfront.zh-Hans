---
title: 创建工作区
description: 工作区是团队使用的操作记录类型和分类的集合，表示团队的工作生命周期。 您可以在Maestro中完全自定义工作区。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 创建工作区

{{maestro-important-intro}}

在Adobe大师中，工作区是团队计划工作的集中位置。

工作区是团队使用的操作记录类型和分类的集合，表示团队的工作生命周期。 您可以在Maestro中完全自定义工作区。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>新增：标准</p>
   <p>当前：计划</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro没有访问级别控制</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>您将获得所创建工作区的管理权限。 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您必须将Maestro区域添加到布局模板中。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

有关访问要求的详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关工作区的注意事项

* 您可以为组织内的特定组织单位创建工作区，以匹配每个单位独特的工作方式。
* 工作区包含的记录类型和分类应反映组织单位的工作生命周期。
* 在创建工作区时，只有您才有权访问和管理工作区。 您必须与其他用户共享，他们才能在同一空间与您协作。 有关信息，请参阅 [共享工作区](/help/quicksilver/maestro/access/share-workspaces.md).
* 您的组织中最多可以有1,000个工作区。
* 工作区包含每个工作区特有的记录类型。 <!--this might change-->

## 创建工作区

{{step1-to-maestro}}

1. （视情况而定）如果您的环境中没有任何工作区，请单击 **创建工作区**

   或者，从现有工作区中，单击工作区名称右侧的向下指向，然后单击 **创建工作区**.

   ![](assets/workspace-drop-down-right-menu.png)

   这将打开Maestro的“工作区”区域。
1. （可选且视情况而定）单击 **预览** 在以下任何预定义workspace模板中：

   * 营销管理
   * 销售管理
   * 产品管理

   指示与每个模板关联的操作记录类型、分类以及字段数。

   ![](assets/previewing-a-workspace-template.png)

   有关Maestro工作区模板的信息，请参阅 [工作区模板列表](../architecture/workspace-templates.md).

1. 单击 **使用模板** 以开始从所选模板创建工作区

   或

   单击 **创建工作区** 从头开始创建工作区。

   将创建以下工作区类型之一：

   * 一个空工作区，您可以在其中开始手动添加记录类型。
   * 填充了示例记录类型的工作区，您可以进一步自定义这些类型。

1. 单击新工作区标题中工作区的名称以对其进行重命名，然后按Enter键

   或

   单击 **更多** 菜单 ![](assets/more-menu.png)工作区名称右侧，然后单击 **重命名**.

1. （可选）单击 **添加记录类型** 向工作区添加记录类型。

   有关信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

1. （可选）单击 **添加分类** 向工作区中添加分类。

   有关信息，请参阅 [创建分类](../architecture/create-a-taxonomy.md).

---
title: 创建工作区
description: 工作区是团队使用的操作记录类型和分类的集合，表示团队的工作生命周期。 您可以在Maestro中完全自定义工作区。
hidefromtoc: true
hide: true
source-git-commit: 6e219089f68db651f5eb8369e3c6df83b6cd823b
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 创建工作区

>[!IMPORTANT]
>
>目前，AdobeMaestro是封闭测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

在Adobe大师中，工作区是团队计划工作的集中位置。

工作区是团队使用的操作记录类型和分类的集合，表示团队的工作生命周期。 您可以在Maestro中完全自定义工作区。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
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
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

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
* 创建工作区时，组织中的所有人都可以查看、编辑或删除该工作区。  <!--this will change with access levels and permissions-->
* 您的组织中最多可以有1,000个工作区。
* 工作区包含每个工作区特有的记录类型。 <!--this might change-->

## 创建工作区

1. （视情况而定）如果系统中没有任何工作区，请单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   或者，从现有工作区中，单击工作区名称右侧的向下指向，然后单击 **创建工作区**.

   ![](assets/workspace-drop-down-right-menu.png)

   这将打开Maestro的“工作区”区域。
1. （可选且视情况而定）单击 **预览** 在以下任何预定义workspace模板中：

   * 营销管理
   * 销售管理
   * 产品管理

   指示与每个模板关联的操作记录类型、分类以及字段数。

   ![](assets/previewing-a-workspace-template.png)

   有关Maestro工作区模板的信息，请参阅 [工作区模板列表](../architecture-and-fields/workspace-templates.md).

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

   有关信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

1. （可选）单击 **添加分类** 向工作区中添加分类。

   有关信息，请参阅 [创建分类](../architecture-and-fields/create-a-taxonomy.md).
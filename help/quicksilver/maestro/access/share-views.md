---
title: 共享视图
description: 在Adobe Workfront Maestro中工作时，您可以与其他人共享视图以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 1%

---


<!--*****************ADD TO TOC AND MINITOC WHEN RELEASING*********************-->

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# 共享视图

在Adobe Workfront Maestro中工作时，您可以与其他人共享视图以确保协作。

向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。

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
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> Adobe大师没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td> <p>管理视图的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须将Maestro区域添加到您的布局模板中。 </p>  
</td>
  </tr>
 </tbody>
</table>

## 共享对视图的权限

您可以共享您创建的视图或您对其具有管理权限的视图。

>[!NOTE]
>
>系统管理员无法查看或共享他们自己未创建的视图。 他们只能查看或共享与其共享的视图。


要与他人共享视图，请执行以下操作：

{{step1-to-maestro}}

1. 打开要共享其视图的工作区，然后单击“记录类型”信息卡。

   这将打开记录类型页面。

1. 在视图下拉菜单中，将鼠标悬停在要共享的视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 视图名称的右侧，然后单击 **共享**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. 在 **授予查看权限** 字段中，开始键入用户或组的名称，然后在列表中显示该名称或组时单击该名称。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 管理

     有关权限级别以及用户可以在每个级别执行的操作的信息，请参阅 [在Adobe大师中共享权限概述](../access/sharing-permissions-overview.md).
1. 单击&#x200B;**保存**。


## 删除视图的权限


{{step1-to-maestro}}

1. 打开要共享其视图的工作区，然后单击“记录类型”信息卡。

   这将打开记录类型页面。

1. 在视图下拉菜单中，将鼠标悬停在要共享的视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 视图名称的右侧，然后单击 **共享**.

1. 查找要删除的用户或组，然后单击 **移除** 用户或组名称右侧的“权限”下拉菜单中。

1. 单击&#x200B;**保存**。

   属于已删除组的用户或用户不再具有查看权限。
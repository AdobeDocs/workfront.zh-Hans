---
title: 共享工作区
description: 在Adobe Workfront Maestro中工作时，您可以与其他人共享工作区以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 50e6b09d626325ee2836dc0ebaf79fc1e8cc9da9
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---


<!--*****************ADD TO TOC AND MINITOC WHEN RELEASING*********************-->

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# 共享工作区

在Adobe Workfront Maestro中工作时，您可以与其他人共享工作区以确保协作。

>[!NOTE]
>
>向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。 有关信息，请参阅 [共享视图](/help/quicksilver/maestro/access/share-views.md).


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
   <td> <p>管理工作区的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须将Maestro区域添加到您的布局模板中。 </p>  
</td>
  </tr>
 </tbody>
</table>

## 共享对工作区的权限

以下用户可以与其他用户共享工作区：

* 系统管理员可以共享所有工作区，包括他们未创建的工作区。
* 所有其他用户只能共享他们对其具有管理权限的工作区。

要与他人共享工作区，请执行以下操作：

{{step1-to-maestro}}

1. 打开要共享的工作区，然后单击 **共享** 屏幕右上角的。

   ![](assets/share-button-on-workspace-top-right.png)

1. 在 **授予工作区访问权限至** 字段中，开始键入用户或组的名称，然后在列表中显示该名称或组时单击该名称。

   ![](assets/sharing-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 参与
   * 管理

     有关权限级别以及用户可以在每个级别执行的操作的信息，请参阅 [在Adobe大师中共享权限概述](../access/sharing-permissions-overview.md).
1. 单击&#x200B;**保存**。


## 删除对工作区的权限


{{step1-to-maestro}}

1. 打开要删除其权限的工作区，然后单击 **共享** 屏幕右上角的。
1. 单击用户或组名右侧的下拉菜单，然后单击 **移除**.
1. 单击&#x200B;**保存**。

   属于已删除组的用户或用户无权再访问工作区或其对象。
---
title: 共享工作区
description: 在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 2%

---


<!--update the metadata and description when we turn this article live; also, update title after Bob adds Planning as a product ??-->

# 共享工作区

{{planning-important-intro}}

在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。

>[!NOTE]
>
>向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。 有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。


## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
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
   或
   <p>当前：计划 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> Adobe Workfront Planning没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p> 
</td>
  </tr>
 </tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享对工作区的权限

以下用户可以与其他用户共享工作区：

* 系统管理员可以共享所有工作区，包括他们未创建的工作区。
* 所有其他用户只能共享他们对其具有管理权限的工作区。

要与他人共享工作区，请执行以下操作：

{{step1-to-planning}}

1. 打开要共享的工作区，然后单击屏幕右上角的&#x200B;**共享**。

   ![](assets/share-button-on-workspace-top-right.png)

1. 在&#x200B;**向**&#x200B;授予工作区访问权限字段中，开始键入用户或组的名称，然后当该名称或组显示在列表中时单击它。

   ![](assets/sharing-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 参与
   * 管理

     有关权限级别以及用户可以针对每个级别执行的操作的信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
1. 单击&#x200B;**复制链接**&#x200B;以将指向工作区的链接复制到剪贴板。
1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问工作区。
1. 单击&#x200B;**保存**。


## 删除对工作区的权限


{{step1-to-planning}}

1. 打开要删除权限的工作区，然后单击屏幕右上角的&#x200B;**共享**。
1. 单击用户或组名称右侧的下拉菜单，然后单击“**删除**”。
1. 单击&#x200B;**保存**。

   属于已删除组的用户或用户无权再访问工作区或其对象。
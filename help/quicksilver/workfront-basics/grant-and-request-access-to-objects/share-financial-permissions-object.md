---
title: 共享对象的财务权限
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑财务数据的权限。 有关详细信息，请参阅授予对财务数据的访问权限。
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 共享对象的财务权限

在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑财务数据的权限。 有关详细信息，请参阅[授予对财务数据的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定项目、任务或问题的财务的权限。

有关每个访问级别中的用户可以如何处理财务数据的信息，请参阅[适用于每个对象类型的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)一文中的[财务数据](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)部分。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>规划</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的项目、任务、问题和财务数据</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看至少包含查看财务权限的项目、任务和问题的权限或更高</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享对象并授予财务权限

向对象授予财务权限时，请考虑以下事项：

* 您可以向项目、任务和问题授予财务权限。
* 权限可以继承：如果您拥有项目的“查看财务”权限，则您会自动继承项目上任务和问题的“查看财务”权限。

要授予对象的财务权限，请执行以下操作：

1. 转到要与他人共享的任务、项目或问题。
1. 在对象名称附近，单击“更多”菜单![](assets/more-icon.png)，然后单击&#x200B;**共享**。

1. 在&#x200B;**授予`<Object name>`对**&#x200B;的访问权限字段中，开始键入要与其共享对象的用户、团队、角色、组或公司的名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 如果所选名称的右侧出现下拉菜单，请单击以下可用选项之一：

   * **查看它**
   * **参与其中**
   * **管理它**

1. 在同一下拉菜单中，单击&#x200B;**高级设置**，然后执行以下操作之一：

   * 如果您在上一步中选择了三个选项之一，请确保已选择&#x200B;**查看财务**。
   * 如果您在上一步中选择了&#x200B;**管理财务**，请确保已选择&#x200B;**管理财务**。

1. 单击&#x200B;**保存**。

## 所有共享级别的财务权限

下表显示了用户在授予他们查看权限、参与权限或管理对象权限时获得的财务权限： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>参与</strong> </th> 
   <th><strong>查看</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>管理开票记录</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看角色计费和成本率</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看用户计费和成本率</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看财务状况</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td>在资源计划工具中按成本查看信息</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>资源规划工具中的预算资源*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在资源计划工具中查看资源*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;需要额外的资源管理权限。

有关资源管理访问权限的信息，请参阅[授予对资源管理的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

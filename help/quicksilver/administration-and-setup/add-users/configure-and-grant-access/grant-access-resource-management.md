---
title: 授予对资源管理的访问权限
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中资源管理的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# 授予对资源管理的访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对资源管理的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定义访问级别配置用户对资源管理工具的访问权限

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 或 **编辑** 按钮，然后选择要在下授予的功能 **优化设置**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在“规划者”中编辑优先级和预算小时数</td> 
      <td> <p>允许具有此许可证的用户执行以下操作：</p> <p>在资源计划器中对项目进行优先级排序。</p> <p>在“资源计划”工具中为资源分配预算（在项目的业务案例中为“资源计划员”和“资源预算”部分）。</p> <p>默认情况下，此选项处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理资源池</td> 
      <td> <p>允许具有此许可证的用户创建、编辑和删除资源池。 默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>在工作负载均衡器中更新已计划的小时数</span> </td> 
      <td> <p>允许具有此许可证的用户在更新负载平衡器中的用户分配时更新工作项目的计划小时数。 分配的小时总数将变为工作项的计划小时数。</p> <p>默认情况下，此选项处于禁用状态。</p> <p> 有关更多信息，请参阅 <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">在工作负载平衡器中管理用户分配</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

   创建访问级别后，您可以将其分配给用户。 有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按许可证类型访问资源管理

有关每个访问级别中的用户可以使用资源管理执行的操作的信息，请参阅部分 [资源管理](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 访问共享问题

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

当您与其他用户共享某个对象时，收件人预算或查看该对象上的资源分配权限由3项内容的组合决定：

* 资源管理的收件人的访问级别设置
* 用户对金融数据的访问权限，如 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* 共享者为对象授予的对财务数据的任何权限

有关用户在共享对象时可以向对象上的财务数据授予权限的信息，请参阅 [共享对象的财务权限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

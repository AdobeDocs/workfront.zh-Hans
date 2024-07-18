---
product-area: projects
navigation-topic: financials
title: 用公司级别的记帐费率覆盖项目级别的记帐费率
description: 用公司级别的记帐费率覆盖项目级别的记帐费率
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 用公司级别的记帐费率覆盖项目级别的记帐费率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

您可以将项目配置为使用公司级别的记帐费率，而不是项目级别的记帐费率。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理具有管理财务权限的项目权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 启用公司级别的记帐费率覆盖选项

当公司与项目相关联并且启用此选项时，对公司级别记帐费率所做的更改将覆盖在项目上设置的记帐费率。

当用户手动重新计算项目财务时，将应用对公司级别记帐费率的任何更改。 历史收入计算也会被覆盖，除非将它们标记为已记帐。

1. 转到项目。
1. 单击标题中项目名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**编辑**。
1. 在&#x200B;**财务**&#x200B;部分中，启用&#x200B;**允许公司级别的记帐费率以覆盖项目级别的记帐费率**。

   >[!CAUTION]
   >
   >启用此选项将覆盖历史收入计算，除非将它们标记为已记帐。 您可以通过创建开票记录来保留历史收入计算。 有关详细信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 单击&#x200B;**保存更改**。

## 更新公司级别的记帐费率并将其应用于项目

在项目上启用了公司级别记帐费率覆盖选项后，对公司记帐费率所做的更改将在任何重新计算财务时应用于项目。

>[!NOTE]
>
>用户必须有权访问其访问级别的公司，才能更新公司级别的记帐费率。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置**。
1. 单击&#x200B;**公司**。
1. 单击与您启用了公司级别记帐费率覆盖的项目关联的公司的名称。
1. 单击左侧面板中的&#x200B;**记帐费率**。
1. 更新现有工作角色的&#x200B;**公司记帐费率**&#x200B;和开始/结束日期，然后按Enter。

   要添加新的生效日期的公司记帐费率，请选择工作角色的记帐费率，然后单击&#x200B;**编辑**。 有关生效日期的公司记帐费率的详细信息，请参阅[覆盖公司级别的工作角色记帐费率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)。

1. 要更新一个或多个项目的公司费率，请执行下列操作之一：

   * 多个项目：

      1. 转到项目列表。
      1. 选中与要更新的项目对应的复选框。
      1. 单击&#x200B;**编辑**。
      1. 在“设置”部分中，启用&#x200B;**重新计算成本和收入**&#x200B;选项。
      1. 单击&#x200B;**保存更改**。

   * 单个项目：

      1. 转到为其启用了公司级别记帐费率覆盖的项目。
      1. 单击标题中项目名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**重新计算财务**。

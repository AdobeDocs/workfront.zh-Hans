---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 设置汇率
description: 作为Adobe Workfront管理员，您可以在Workfront中设置货币汇率。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# 设置汇率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作为Adobe Workfront管理员，您可以在Workfront中设置货币汇率。 这包括以下内容：

* 设置Workfront系统的默认货币
* 在Workfront中更新汇率以匹配当前汇率
* 为多种货币配置汇率（这样做可让用户为各个项目选择默认货币）

汇率影响Workfront的所有金融元素。 基本货币是整个系统中所有项目的默认货币，除非为给定项目或工作角色覆盖基本货币。 在报表或列表中查看财务信息时，您也可以选择以系统中可用的货币显示财务信息，这些货币与项目的基本货币或项目的基本货币不同。 有关详细信息，请参阅[创建具有唯一汇率的财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

有关在Workfront中为项目和工作角色覆盖基本货币的更多信息，请参阅以下文章：

* [更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md)
* [创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

设置汇率的方式会影响用户是否可以修改给定项目的汇率。

>[!IMPORTANT]
>
>Workfront中的汇率不是动态的；在汇率发生更改时，必须更新您设置的值。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置汇率

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **汇率。**

1. 单击&#x200B;**添加货币。**
1. 开始键入货币的名称，然后在货币出现在下拉列表中时单击该货币。

1. 在提供的字段中，指定所选货币的汇率，因为该汇率与系统中设置为基础货币的货币相关。
1. （可选）将货币设置为Workfront的基本（默认）货币。

   该货币用作整个系统所有项目和报表的默认货币。

1. 单击&#x200B;**保存**&#x200B;以保存更改。

## 允许用户修改项目的默认货币

在满足以下条件时，用户可以修改项目的默认货币：

* 用户拥有对汇率具有管理访问权限的计划许可证。

  有关详细信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系统上启用了多种货币。

有关用户如何更改给定项目的默认货币的信息，请参阅[更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 允许用户修改工作角色的默认货币

在满足以下条件时，用户可以修改工作角色的货币：

* 用户拥有对工作角色具有管理访问权限的计划许可证。

  有关详细信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系统中启用了多种货币。

有关用户如何更改给定工作角色的默认货币的信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

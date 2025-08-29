---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 设置汇率
description: 汇率影响Workfront的所有金融元素。 基础货币是整个系统中所有项目的默认货币。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '650'
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

汇率影响Workfront的所有金融元素。 基础货币是整个系统中所有项目的默认货币，除非为给定项目或工作角色覆盖基础货币。 当前的基本货币或默认货币在列表中以图标![默认货币图标](assets/default-icon.png)表示。 在报表或列表中查看财务信息时，您也可以选择以系统中可用的货币显示财务信息，这些货币与项目的基本货币或项目的基本货币不同。 有关详细信息，请参阅[创建具有唯一汇率的财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

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
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置汇率

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **汇率**。

1. 单击&#x200B;**添加货币**。
1. 在&#x200B;**添加货币**&#x200B;框中，开始键入货币的名称，然后当它出现在下拉列表中时单击它。
1. 在&#x200B;**汇率**&#x200B;字段中，输入所选货币与系统中设置为基础货币的货币之间的汇率。
1. 单击&#x200B;**添加**&#x200B;以添加新货币及其汇率。
1. （可选）要更改基本（默认）货币，请执行下列操作之一：

   * 选中货币名称旁边的复选框，然后在屏幕底部的操作栏中选择&#x200B;**设为默认值**。
   * 将鼠标悬停在货币名称上，然后单击显示的&#x200B;**更多**&#x200B;菜单。 然后，选择&#x200B;**设为默认值**。

     新的默认货币会更新为图标。

     >[!NOTE]
     >
     >无论列表如何排序，默认货币始终显示在列表中的第一个位置。

1. （可选）要删除货币，请选中货币名称旁边的复选框，然后在屏幕底部的操作栏中选择&#x200B;**删除**。 不能删除默认货币。

## 允许用户修改项目的默认货币

在满足以下条件时，用户可以修改项目的默认货币：

* 用户拥有对汇率具有管理访问权限的“标准”或“计划”许可证。

  有关详细信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系统上启用了多种货币。

有关用户如何更改给定项目的默认货币的信息，请参阅[更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 允许用户修改工作角色的默认货币

在满足以下条件时，用户可以修改工作角色的货币：

* 用户拥有对工作角色具有管理访问权限的标准或计划许可证。

  有关详细信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系统中启用了多种货币。

有关用户如何更改给定工作角色的默认货币的信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->

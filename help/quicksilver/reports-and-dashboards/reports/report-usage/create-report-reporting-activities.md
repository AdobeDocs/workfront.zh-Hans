---
product-area: reporting
keywords: 更改，所有者，共享，报表，共享，运行，用户，访问，权限，已输入，上次，已查看，日期，报表，活动
navigation-topic: report-usage
title: 创建报告活动报告
description: 在创建有关报表的报表时，您可以标识特定的报表信息，这些信息包括：是否将报表分配给已停用的用户；是否将报表设置为使用已停用用户的访问权限运行；用户是否访问您计划删除的报表，等等。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 创建报告活动报告

在创建有关报表的报表时，您可以标识特定的报表信息，这些信息包括：是否将报表分配给已停用的用户；是否将报表设置为使用已停用用户的访问权限运行；用户是否访问您计划删除的报表，等等。

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 创建有关现有报表的报告 {#create-the-report-about-existing-reports}

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。
1. 单击&#x200B;**报表**，然后单击&#x200B;**新建报表**。
1. 在&#x200B;**新建报表**&#x200B;下拉菜单中，选择&#x200B;**报表**&#x200B;以创建现有报表的报告。

1. 在&#x200B;**列（视图）**&#x200B;选项卡中，在报表中添加所需的列。\
   以下某些字段可能很有用：

   | 字段 | 描述 |
   |---|---|
   | **作为用户运行：名称** | 这是在&#x200B;**使用此报告上的**&#x200B;字段的访问权限运行此报告中指定的用户。 如果未激活此用户，则不会为与该用户共享该报表的任何人显示报表。 |
   | **共享对象：** | 这些是与报告共享的所有实体。 |
   | **输入者** | 这是报告的所有者。 |
   | **上次查看日期** | 这是用户上次查看报告的日期和时间。 |

   {style="table-layout:auto"}

1. （可选）要将报表列表限制为仅列出特定的已停用用户，请执行以下操作：

   1. 选择&#x200B;**筛选器**&#x200B;选项卡，然后单击&#x200B;**添加筛选器规则**。

   1. 添加筛选器&#x200B;**以用户ID** > **等于**&#x200B;身份运行。

   1. 键入要添加到筛选器的已停用用户的名称，然后在列表中显示该名称时单击该名称。
   1. 重复步骤C，直到选择了所有要包含在报表中的已停用用户。

1. （可选）要将报表列表限制为计划报表，请执行以下操作：

   1. 选择&#x200B;**筛选器**&#x200B;选项卡，然后单击&#x200B;**添加筛选器规则**。

   1. 添加筛选器&#x200B;**计划报表ID** > **不为空**。

1. 单击&#x200B;**保存+关闭**，然后键入报告的名称，然后单击&#x200B;**保存报告**。

   此时会显示您的报表信息。

1. （可选）将此报表导出到Excel并将其保存在计算机上。\
   有关导出报告的信息，请参阅[导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 更新有关报告的信息

创建报告后，您可以根据需要更新报告。

1. 转到要更新的报告。
1. 根据您要执行的操作，执行以下操作之一：

   * 将&#x200B;**访问权限为**&#x200B;的字段运行此报告更新给活动用户：有关详细信息，请参阅[运行并交付一个访问权限为其他用户的报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)。

   * 创建报告副本：有关详细信息，请参阅[创建报告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。
   * 删除报告：有关详细信息，请参阅文章[创建报告的副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)的[创建报告的精确副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2)部分。

   * 共享报告：有关详细信息，请参阅[在Adobe Workfront中共享报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

1. （视情况而定）如果复制原始报告，请使用您在[中创建的报告中的信息创建关于现有报告的报告](#create-the-report-about-existing-reports)，以便与原始报告相同的实体共享新副本。

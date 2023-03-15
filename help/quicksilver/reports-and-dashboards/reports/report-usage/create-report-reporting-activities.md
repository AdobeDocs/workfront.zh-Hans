---
product-area: reporting
keywords: 更改，所有者，共享，报表，共享，运行，用户，访问，权限，输入，上次，查看，日期，报告，活动
navigation-topic: report-usage
title: 创建报告活动报告
description: 在创建有关报表的报表时，您可以识别特定的报表信息，这些信息包括如果将报表分配给已停用的用户，如果将报表设置为使用已停用用户的访问权限运行，或者如果用户正在访问您计划删除的报表，等等。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# 创建报告活动报告

在创建有关报表的报表时，您可以识别特定的报表信息，这些信息包括如果将报表分配给已停用的用户，如果将报表设置为使用已停用用户的访问权限运行，或者如果用户正在访问您计划删除的报表，等等。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建有关现有报表的报表 {#create-the-report-about-existing-reports}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击 **报表**，则 **新建报表**.
1. 在 **新建报表** 下拉菜单，选择 **报表** 创建现有报表的报表。

1. 在 **列（视图）** 选项卡上，添加您希望在报表中使用的列。\
   以下某些字段可能很有用：

   | 字段 | 描述 |
   |---|---|
   | **以用户身份运行：名称** | 这是 **使用以下访问权限运行此报表：** 字段。 如果此用户已停用，则不会向与其共享报表的任何人显示报表。 |
   | **共享对象** | 这些是与报表共享的所有实体。 |
   | **输入者** | 这是报表的所有者。 |
   | **最近查看日期** | 这是用户上次查看报表的日期和时间。 |

   {style="table-layout:auto"}

1. （可选）要将报表列表限制为特定已停用用户，请执行以下操作：

   1. 选择 **过滤器** ，然后单击 **添加过滤器规则**.

   1. 添加过滤器 **以用户ID身份运行** > **等于**.

   1. 键入要添加到过滤器的已停用用户的名称，然后在列表中显示该名称时单击该名称。
   1. 重复步骤C，直到您选择了要包含在报表中的所有已停用用户。

1. （可选）要将报表列表限制为计划报表，请执行以下操作：

   1. 选择 **过滤器** ，然后单击 **添加过滤器规则**.

   1. 添加过滤器 **计划报表ID** > **不为空**.

1. 单击 **保存并关闭**，然后键入报表的名称，并单击 **保存报表**.

   此时会显示您的报表信息。

1. （可选）将此报表导出到Excel，并将其保存在您的计算机上。\
   有关导出报表的信息，请参阅 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## 更新有关报表的信息

创建报表后，您可以根据需要更新报表。

1. 转到要更新的报表。
1. 根据您要执行的操作，执行以下操作之一：

   * 更新 **使用以下访问权限运行此报表：** 字段：有关更多信息，请参阅 [运行并提交具有其他用户访问权限的报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * 创建报表副本：有关更多信息，请参阅 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * 删除报表：有关详细信息，请参阅 [创建报表的确切副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) 文章一节 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * 共享报表：有关更多信息，请参阅 [在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. （视情况而定）如果您复制原始报表，请使用您在中创建的报表中的信息 [创建有关现有报表的报表](#create-the-report-about-existing-reports) 将新副本与原始报表的相同实体共享。

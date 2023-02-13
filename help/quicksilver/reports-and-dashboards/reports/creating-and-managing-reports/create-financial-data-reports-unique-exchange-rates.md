---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 使用独特的汇率创建财务数据报表
description: 如果在Adobe Workfront中配置了多个汇率，则可以在报表和列表中将财务值设置为以默认货币以外的货币显示。
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# 使用独特的汇率创建财务数据报表

如果在Adobe Workfront中配置了多个汇率，则可以在报表和列表中将财务值设置为以默认货币以外的货币显示。

>[!IMPORTANT]
>
>如果在视图中选择默认货币以外的货币，则不会再看到链接 **添加更多任务** 和 **添加更多问题** 项目列表底部。

有关如何更改给定项目的默认货币的信息，请参阅 [更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md).

如果报表中存在使用单一货币的项目，则分组中的总和也将以系统默认货币显示。

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

## 先决条件

在您查看本节所述的替代货币之前，Workfront管理员必须先在Workfront的“设置”区域中启用并配置多个货币。 有关信息，请参阅 [设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## 将财务值应用于报表 {#apply-financial-values-to-a-report}

要在处理报表时在货币之间转换财务值，请执行以下操作：

1. 转到要将财务值换算为其他货币的报表。
1. 单击 **查看** 下拉列表中，单击 **更改货币**，然后选择要在中显示财务值的以下货币之一：

   * 项目的原始货币
   * 任何其他货币

      >[!TIP]
      >
      >您只能选择之前在“设置”中选择的货币。
   通过使用此选项，您可以在汇率值之间快速转换报表中的财务值。

   ![更改货币](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## 在具有不同货币的多个项目中显示默认货币

当您在项目级别自定义货币，并且希望显示同一报表中所有项目的信息时，会出现以下情况：

* 如果创建的报表从应用了不同货币的两个或更多项目中收集财务信息，则默认情况下，分组摘要会反映Workfront管理员选择的系统默认货币。
* 如果您为两个或更多具有相同货币但与系统默认货币不同的项目创建报表，则分组中的总和将使用系统默认货币显示。
* 如果您为两个或多个具有与货币改写相关联的职务角色分配的项目创建报表，则Workfront会将财务信息从职务角色的已改写货币汇率换算为项目的货币（在视图中选择项目的原始货币时），或换算为查看报表时选择的任何其他货币。 有关覆盖职务角色货币的信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

要在报表中显示两个具有自定义货币的项目，请执行以下操作：

1. 创建应用不同货币的两个项目。

   ![](assets/qs-currency-350x217.png)

1. 记录两个项目的小时数。

   有关记录时间的更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，然后单击 **报表**.
1. 单击 **新建报表**，则 **项目报表**.
1. 在 **列（视图）** 选项卡，添加 **实际成本** 列和汇总方式 **总和**.

   有关如何创建列的信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 在 **分组** 选项卡，应用 **计划完成日期** 分组。

   有关如何创建分组的信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. 在 **过滤器** 选项卡，为 **项目名称** 并选择两个不同货币的项目。

   有关如何创建过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 单击 **保存并关闭**.

   总计 **实际成本** 会使用系统默认货币在分组中显示，而不考虑报表中项目的货币。

   ![分组中显示的货币](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   如果两个项目具有不同的货币，则系统默认货币也会显示在报表的分组中。

## 在项目级别的报表中显示项目货币

如果对项目中的任务或小时列表应用分组，则分组中的总和将以项目的货币显示。

1. 使用与系统默认货币不同的自定义货币创建项目。
1. 转到项目，并确保其中包含已记录任务的小时数。

   有关记录时间的更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >应将任务分配给具有每小时费率的用户或作业角色。

1. 单击 **任务**.
1. 展开 **查看** 下拉菜单，然后选择 **新建视图**.
1. 添加 **实际成本** 在新的“视图为新列”中，并通过 **总和**.
1. 单击 **完成**，然后单击 **保存视图**.
1. 展开 **分组** 下拉菜单，然后选择 **新建分组**.
1. 添加 **实际完成日期** 在作为新字段的新分组中，单击 **保存分组**.

   的 **实际成本** 列在新的分组中进行汇总，并以项目的货币显示总计。

## 编辑具有唯一货币的报表

在您更改报表设置以显示项目的原始货币之前，报表中的财务字段不可编辑。

要在报表中内嵌编辑财务字段，请执行以下操作：

1. 导航到报表。

   >[!NOTE]
   >
   >如果默认货币未在任何其他区域中为列表显示，则可以编辑“视图”以显示默认货币。\
   >有关如何在视图中更改货币的信息，请参阅本文中的部分 [将财务值应用于报表](#apply-financial-values-to-a-report).

1. 单击 **报表操作**，然后选择 **编辑**.
1. 单击 **报表设置**.
1. 单击 **默认货币** 下拉列表，然后选择 **项目的原始货币**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. 单击 **完成**.

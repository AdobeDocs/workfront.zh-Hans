---
product-area: resource-management
navigation-topic: resource-planning
title: 使用Adobe Workfront资源计划员复查资源可用性和分配
description: 您可以在资源计划器中查看资源的可用性以及项目的计划或预算工作量。 这些值以小时、FTE（等效全职）或成本金额显示，并按列进行组织。
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 4%

---

# 使用Adobe Workfront资源计划员复查资源可用性和分配

您可以在资源计划器中查看资源的可用性以及项目的计划或预算工作量。 这些值以小时、FTE（等效全职）或成本金额显示，并按列进行组织。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问以下内容：</p> 
    <ul> 
     <li> <p>资源管理</p> </li> 
     <li> <p>财务数据</p> </li> 
     <li> <p>用户</p> </li> 
     <li> <p>项目</p> </li> 
    </ul> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在资源计划器中查看要查看的项目的查看权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## 先决条件

您必须满足使用资源计划员所需的所有先决条件。 有关更多信息，请参阅 [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>如果缺少资源计划员正确功能所需的任何先决条件，则某些数字可能为零，或预算小时数可能变暗。

## 资源的可用性和分配

显示资源可用性和分配的列会根据您应用到资源计划员的视图而发生更改。 有关按项目、职责或用户显示资源计划员中信息的信息，请参阅 [资源计划员导航概述](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

在将视图更改为资源计划员时，请考虑以下事项：

* 当您应用 **按项目查看** 或&#x200B;**按角色查看** 视图，您可以看到以下列：

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * 可用小时数、FTE或成本
   * 计划小时数、FTE或成本
   * 预算小时数、FTE或成本
   * 小时数、FTE或成本差异
   * 净小时数、FTE或成本

* 当您应用 **按用户查看** 视图，您可以看到以下列：

   * 可用小时数或FTE
   * 计划小时数或FTE
   * 小时或FTE差异
   * 计划小时分配百分比

>[!TIP]
>
>在应用 **按用户查看** 查看资源计划员。
>
>有关每列显示内容的更多信息，请将鼠标悬停在显示数字的列的名称上。\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>有关每列中显示数据的更多信息，请参阅以下文章：
>
>* [资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [使用“用户”视图时，在资源计划器中查看可用、计划和实际工时或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## 按小时、FTE或成本查看信息

1. 转至资源计划员。

   默认情况下，信息按小时在资源计划器中显示。

1. 展开下拉菜单。\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. 从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">小时</td> 
      <td>以小时为单位显示可用性和分配信息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>显示FTE中的可用性和分配信息。</p> <p>有关如何在资源计划器中计算FTE的详细信息，请参阅 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">资源计划员中用户和角色的小时数和FTE计算概述</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本</td> 
      <td> <p>如果您在“项目”或“职责”视图中查看资源计划员，则按成本显示可用性和分配信息。 该信息会以系统的货币显示值。 您的Workfront管理员定义系统货币。 有关在Workfront中设置系统货币的更多信息，请参阅 <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> <p><b>注释</b>

   您必须将用户和任务职责与每小时成本费率关联，以便在资源计划器中显示成本信息。<br style="font-style: italic;">有关将每小时成本费率与任务职责关联的详细信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.<br style="font-style: italic;">有关将每小时成本费率与用户关联的详细信息，请参阅 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>.<br style="font-style: italic;">有关如何在资源计划器中计算成本的详细信息，请参阅 <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">在资源计划器中计算成本 </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">自定义</td> 
      <td>创建在资源计划器中显示的列的自定义视图。 按照以下步骤所述，选择要在资源计划器中显示的选项。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您选择 **自定义**，指示 **自定义显示的量度** 框来设置自定义视图。

   ![](assets/planner-customize-view-box-350x114.png)

1. 在 **视图类型** 列中，选择以下视图之一：

   * 项目
   * 角色
   * 用户

1. 在 **显示选定项目** ，选择要在选定视图的列中显示的信息类型。 下表显示了每个视图中可用的选项：

   | **选项** | 用户视图 | 项目视图 | 角色视图 |
   |---|---|---|---|
   | 可用 | ✔ | ✔ | ✔ |
   | 计划 | ✔ | ✔ | ✔ |
   | 已预算 |   | ✔ | ✔ |
   | 差异 |   | ✔ | ✔ |
   | Net |   | ✔ | ✔ |
   | 实际 | ✔ |   |   |
   | 差异 | ✔ |   |   |
   | 百分比 | ✔ |   |   |

1. 选择 **在NET计算中使用计划值(PLN)** 在“项目”和“职责”视图中计算“净值”时，使用“已计划”信息而不是“已预算”信息。

   选择此选项时，Workfront会使用以下公式计算净值：

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**仅当您在“显示选定项目”部分中至少选择一个用于自定义视图的选项时，才应用此选项。**

1. 单击&#x200B;**保存**。

   此时会显示包含您选定列的自定义视图。

   资源计划员在“小时”下拉菜单中将自定义视图列为“自定义”。

   >[!NOTE]
   >
   >您只能有一个自定义视图。

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## 查看用户分配图表

您可以在图表中根据用户的可用性显示计划的分配用户。

要在图表中显示用户分配，请执行以下操作：

1. 转至资源计划员。

   有关访问资源计划员的详细信息，请参阅 [查找资源计划员](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) 章节 [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. 选择 **按用户查看**.

   >[!TIP]
   >
   >您只能在“用户视图”中查看用户分配图表。

1. 单击 **用户分配图表** 图标 ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) 显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有用户都没有过度分配的可用性百分比</td> 
      <td>这是某个时间段内所有用户都可以工作的时间，以其总可用时间的百分比表示。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有用户的过度分配百分比 </td> 
      <td> <p>这是用户在某个时间段内被过度分配的时间，以占总可用时间的百分比表示。</p> <p><b>注释</b>

   当计划小时数大于可用小时数时，会发生超额分配。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">所有用户的低利用率百分比</td> 
      <td> <p>这是用户在某个时间段内未充分利用的时间，以占总可用时间的百分比表示。</p> <p><b>注释</b>

   当计划小时数低于可用小时数时，会出现利用率不足的情况。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">在此期间，至少过度分配了一个用户</td> 
      <td>这表示在一个时间段内至少有一个用户存在过度分配，尽管在该时间段内所有用户的总时间没有过度分配。<br>您必须滚动浏览用户列表，而被过度分配的用户的小时数将以红色突出显示。</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. （可选）单击 **所有用户的超额分配百分比** 的上界。\
   所有过分配的用户都以红色突出显示。
1. （可选）单击 **所有用户的利用率不足%** 的上界。\
   所有未充分利用的用户都以蓝色突出显示。

1. （可选）单击指示器图标 ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) 显示您至少有一个用户被过度分配的位置。\
   被过度分配的用户以红色突出显示。

1. （可选）刷新页面以折叠图表。

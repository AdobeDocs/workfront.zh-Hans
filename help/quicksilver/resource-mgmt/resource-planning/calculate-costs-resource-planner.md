---
product-area: resource-management
navigation-topic: resource-planning
title: 在资源规划者中计算成本
description: 您可以在Adobe Workfront资源规划程序中通过使用成本值（而不是小时或FTE值）来预算资源。 成本值不适用于资源规划者中的**按用户查看**视图。
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---

# 在资源规划者中计算成本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

您可以在Adobe Workfront资源规划程序中通过使用成本值（而不是小时或FTE值）来预算资源。 资源规划者中的&#x200B;**按用户查看**&#x200B;视图的成本值不可用。

>[!IMPORTANT]
>
>您必须将用户和工作角色与每小时成本费率关联，以便在资源规划者中显示成本信息。\
>有关将每小时成本费率与工作角色关联的详细信息，请参阅[创建和管理工作角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。\
>有关将每小时成本费率与用户关联的详细信息，请参阅[编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

在预算您的资源之前，请确保您充分了解需要完成的工作（计划小时数、FTE或成本）以及用户可工作的时间（可用小时数、FTE或成本）。\
有关在按小时或FTE进行预算时了解资源规划程序中的信息的详细信息，请参阅资源规划程序的项目和角色视图中的[小时概览、FTE和成本信息](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，包括访问资源规划者中的编辑优先级和预算小时数</p> <p>编辑对财务数据、项目和用户的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要为其预算信息的项目的权限，并具有管理财务的能力</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 按成本显示资源规划程序中的信息

默认情况下，可用性和分配信息显示在资源规划者的小时数中。

要在资源规划程序中按成本显示可用、计划和预算信息，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**资源**。
1. 转到资源规划者。
1. （视情况而定）选择&#x200B;**按项目查看**&#x200B;或&#x200B;**按角色查看**。\
   默认情况下，**按项目查看**&#x200B;处于选中状态。\
   分配和可用性信息以小时数显示。

1. 从&#x200B;**小时**&#x200B;下拉菜单中，选择&#x200B;**成本**。

   如果您无权访问访问访问级别中的财务数据，则此选项不可用。\
   如果项目的币种不同于系统币种，则这些项目的成本将以系统币种折换的资源计划员中显示。 系统管理员定义系统货币。\
   有关在Workfront中设置系统货币和转换率的详细信息，请参阅[设置汇率](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## 在资源规划程序中计算可用成本

要在资源计划员中显示可用成本值，您必须具备以下各项：

* 用户和角色的每小时成本费率
* 有关用户可用性的信息。

  获取有关用户可用性的信息取决于Workfront管理员配置资源管理首选项的方式。\
  有关计算用户可用性和设置资源管理首选项的详细信息，请参阅[配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

下表说明了如何在资源计划程序中计算可用成本：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>可用成本</strong> </th> 
   <th><strong>计算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>用户可用成本</td> 
   <td> <p>使用以下公式计算每个用户的可用成本：</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>注释</b>

如果用户在其配置文件中没有每小时成本费率，则在计算中使用列出用户的工作角色的每小时成本费率。 如果用户没有与其关联的角色，则可用用户成本为$0。 </p> </td>
</tr> 
  <tr> 
   <td>角色可用成本</td> 
   <td> <p>每个角色的可用成本使用以下公式计算：</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>注释</b>

如果角色没有每小时成本费率，则可用角色成本为$0。</p> </td>
</tr> 
  <tr> 
   <td>项目可用成本</td> 
   <td> <p>每个项目的可用成本使用以下公式计算：</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 在资源规划者中计算计划成本

虽然您不能在资源规划者中查看任务信息，但可通过考虑以下任务信息来计算用户、角色和项目的计划成本：

* 任务的分配类型。\
  您可以将任务保留为未分配，或将以下实体分配给任务：

   * 用户（无论是否具有工作角色）
   * 角色
   * 一个团队\
     从资源规划者的角度来看，分配给团队的任务被视为未分配。

* 项目任务的&#x200B;**成本类型**。\
  有关任务的成本类型的详细信息，请参阅[跟踪成本](../../manage-work/projects/project-finances/track-costs.md)。

* 工作角色和用户的成本费率的生效日期。

  例如，如果角色或用户在2月有10个计划小时数，在3月有10个计划小时数，但成本率已从3月的12美元更改为20美元，则2月的计划成本值为$120，在3月，计划成本为$200。

>[!NOTE]
>
>用户计划成本不影响项目计划成本。 只有角色计划成本会影响资源规划者中的项目计划成本。

在计算用户、角色和项目的计划成本时，存在以下方案：

* 当&#x200B;**成本类型**&#x200B;为**用户小时**并且任务上有&#x200B;**无分配**&#x200B;时：

   * **角色和用户计划成本**：

     角色和用户计划成本为0.00 USD。

   * **项目计划成本**：

     项目计划成本为$0.00。

* 当&#x200B;**成本类型**&#x200B;为&#x200B;**用户小时**，并且任务中有&#x200B;**用户分配**&#x200B;时：

   * **角色和用户计划成本**：

     使用以下公式计算用户计划成本：

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     如果用户在其配置文件中具有成本费率，则该费率用于计算计划成本。 否则，将使用其主要角色的系统级每小时成本费率。

     >[!NOTE]
     >
     >可以将用户与其辅助工作角色之一分配给任务，但此处改为使用主要工作角色的速率。

     使用以下公式计算职责计划成本：

     `Role Planned Cost = SUM(User Planned Cost)`

   * **项目计划成本**：

     项目计划成本为$0.00。

* 当&#x200B;**成本类型**&#x200B;为&#x200B;**用户小时**，并且任务中有&#x200B;**工作角色分配**&#x200B;时：

   * **角色和用户计划成本**：

     用户计划成本为$0.00。

     使用以下公式计算职责计划成本：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     分配至任务的工作角色的系统级别每小时成本费率用于计算计划成本。

   * **项目计划成本**：

     项目计划成本为$0.00。

* 当&#x200B;**成本类型**&#x200B;为&#x200B;**角色小时**&#x200B;且任务上有&#x200B;**无分配**&#x200B;时：

   * **角色和用户计划成本**：

     角色和用户计划成本为0.00 USD。

   * **项目计划成本**：

     项目计划成本为$0.00。

* 当&#x200B;**成本类型**&#x200B;为&#x200B;**角色小时**，并且任务上有&#x200B;**用户分配**&#x200B;时：

   * **角色和用户计划成本**：

     用户计划成本为$0.00。

     角色计划成本按以下公式计算：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront查看用户在任务中履行的工作角色，以计算该角色的计划成本。

     如果用户未与任务中的任何角色关联，则计划成本为$0.00。

   * **项目计划成本**：

     使用以下公式计算项目计划成本：

     `Project Planned Cost = SUM(Role Planned Costs)`

* 当&#x200B;**成本类型**&#x200B;为&#x200B;**角色每小时**，并且任务中有&#x200B;**工作角色分配**&#x200B;时：

   * **角色和用户计划成本**：

     用户计划成本为$0.00。

     角色计划成本按以下公式计算：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront查看用户在任务中履行的工作角色，以计算该角色的计划成本。

   * **项目计划成本**：

     使用以下公式计算项目计划成本：

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## 在资源规划者中计算预算成本

要在资源计划员中显示预算成本值，您必须具备以下各项：

* 角色、用户和项目的预算小时数。
* 用户和角色的每小时成本。

>[!NOTE]
>
>项目的预算小时数是根据角色的预算小时数计算的，而不是用户的预算小时数。

下表说明了如何在资源规划程序中计算预算成本：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>预算成本</strong> </th> 
   <th><strong>计算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>用户预算成本</td> 
   <td> <p>每个用户的预算成本使用以下公式计算：</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>注释</b>

如果用户档案中没有每小时成本费率，则预算用户成本为$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>角色预算成本</td> 
   <td> <p>角色预算成本使用以下公式计算：</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>注释</b>

如果角色没有每小时成本费率，则预算角色成本为$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>项目预算成本</td> 
   <td> <p>每个项目的预算成本使用以下公式计算：</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>

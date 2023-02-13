---
product-area: resource-management
navigation-topic: resource-scheduling
title: 在“计划”区域中自动分配未分配的任务和问题
description: 使用计划工具时，您可以允许Adobe Workfront分析可用用户中的当前工作分配，并为任何尚未分配的任务或问题建议智能的逻辑分配。 在完成所有建议的分配之前，您可以修改它们。
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# 在“计划”区域中自动分配未分配的任务和问题

>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版本开始，本文中描述的计划功能已弃用并从Adobe Workfront中删除。   </span>
>  
> <span class="preview"> 2023年初23.1版发布后不久，也将删除本文。 此时，我们建议您相应地更新任何书签。 </span>
> 
><span class="preview"> 您现在可以使用负载平衡器来计划资源的工作。 </span>
>  
> <span class="preview">有关使用工作负载平衡器计划资源的信息，请参阅一节 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

使用计划工具时，您可以允许Adobe Workfront分析可用用户中的当前工作分配，并为任何尚未分配的任务或问题建议智能的逻辑分配。 在完成所有建议的分配之前，您可以修改它们。

Workfront会查看当前选定日期范围内“未分配”区域中可用的任务和问题，并一次为每个项目建议分配。 您可以创建过滤器以限制“未分配”区域中可用的项目数。

系统管理员确定Workfront如何在系统级别计算资源可用性（考虑工时和FTE可用性）。 根据此系统范围的设置，可使用默认计划或用户的计划来计算资源可用性。 有关更多信息，请参阅 [配置Workfront如何计算“计划”区域的资源小时数和FTE可用性](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高程度地访问项目、任务和问题</p> <p><strong>注释</strong>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为更新的项目、任务和问题提供权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件 {#prerequisites}

Workfront使用专有算法来确定分配建议书。 为了获得最佳结果，请确保在Workfront中准确提供以下信息：

* 任务和问题信息，包括：

   * 角色分配\
      对于未分配给角色的任务和问题，不提出建议。
   * 计划小时\
      如果任务或问题当前没有计划时间，则Workfront在自动分配工作时假设每个工作日有4个计划时间。 这些小时不会自动分配给工作项目；它们仅用于确保更实际的分配。
   * 计划起始日期和计划完成日期

* 用户信息，包括：

   * 用户配置文件上的主要和次要角色分配
   * 项目团队信息

## 配置角色限制

角色限制可控制具有特定角色的可自动分配工作的用户数量。 角色限制基于每个项目进行工作，以确保基于角色的任务不会分散到大量用户中。

以下方案概述了角色限制如何应用于项目：

* **场景1**:如果没有为项目团队分配用户，则系统将使用角色限制来分配任务。\
   例如，您的项目没有为项目团队分配任何用户。 此项目有10个需要分配的项目管理任务，您为项目经理角色设置了角色限制为1。 由于角色限制设置为1，因此系统会将所有10项任务分配给1个项目经理。

* **场景2**:如果角色限制大于分配给项目团队的用户数，则会为其他用户分配任务。\
   例如，您的项目中为项目团队分配了一个作者。 此项目有12个需要分配的编写器任务，并且您为编写器角色设置了角色限制为2。 由于角色限制设置为2，因此系统会在项目团队编写器和其他编写器之间分配所有12项任务。

* **场景3**:如果角色限制小于分配给项目团队的用户数，则角色限制将被覆盖。\
   例如，您有一个项目，该项目的项目团队分配了4名设计人员。 此项目有8个需要分配的设计人员任务，您为设计人员角色设置了角色限制为2。 即使角色限制设置为2，系统仍会在4个项目团队设计人员中的每个人之间分配所有8个任务。

要设置职务角色分配的限制，请执行以下操作：

1. 转到多个项目或单个项目的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。

1. 单击 **设置** 图标。\
   ![Automode_settings.png](assets/automode-settings.png)

1. 在自动资源计划部分中，单击 **限制** 列中与 **角色** 列，然后输入正数。\
   Workfront会自动保存您所做的更改。

   >[!NOTE]
   >
   >无论设置何种角色限制，所有当前项目团队成员都自动有资格参与所有推荐的工作。

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. （可选）单击 **显示** 菜单，然后选择所需的显示选项。
1. 要返回资源计划区域，请单击 **返回计划**.

## 自动分配任务和问题

无论您是在“计划”选项卡（为多个项目计划资源时）还是“人员配备”选项卡（为单个项目计划资源时），您都可以在计划时间轴上为用户分配任务和问题。

要允许Workfront在“未分配”区域中自动为任务和问题建议分配，请执行以下操作：

1. 转到多个项目或单个项目的计划时间轴：

   * **对于多个项目**:  单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **资源配置>工作负载平衡器**，然后选择 **计划** 中。
   * **对于单个项目**:转到项目，单击 **工作负载平衡器** ，然后选择 **计划** 从左上角的下拉菜单中。

1. （可选）创建过滤器以自定义在计划时间轴上的“未分配”区域中显示的内容。\
   有关创建过滤器的更多信息，请参阅 [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [在“计划”区域中筛选信息](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >要确保Workfront将工作分配给最符合条件的用户，请执行以下操作：
   >
   >* 仅过滤影响“未分配”区域中显示的任务(如Portfolio、程序、项目)的信息。
   >* 我们建议您不要过滤影响可在计划时间轴上分配哪些用户的信息。 这样做会限制Workfront查看所有潜在受让人，这可能会导致分配不满意。


1. （可选）修改计划时间线上显示的日期范围，如 [调整计划区域的日期范围](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [资源计划入门](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront仅在计划时间轴上的可见日期范围内的任务和问题进行分配。

1. 单击 **自动** 按钮。\
   ![scheduling_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront建议为 **未分配** 的上界。

   >[!TIP]
   >
   >必须已将任务和问题分配给角色，才能提议分配。 为确保获得最佳结果，任务和问题应包含 [先决条件](#prerequisites).

   建议的分配在每个任务或问题周围用虚线轮廓区分，如下所示：\
   **拟议任务分配：**

   **现有任务分配：**

1. （可选）在完成分配之前，您可以修改任何建议或现有分配：

   >[!NOTE]
   >
   >如果修改现有分配，则它将变为建议状态。

   * 要将项目分配给其他用户，请执行以下操作：

      * 将任务或问题从建议的用户拖到要分配的其他用户的行中。

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         给定用户每天最多显示10个任务。 您可以展开列表以查看当前分配给该用户的所有任务。 （在计划时间轴上进行分配后，可能会临时显示10个以上的任务。）\
         拖动项目时，会在释放任务或问题并完成分配之前显示以下信息：

         * 用户的行中会显示一个拖放指示器。 这样，您就可以在进行分配之前，查看物料的分配位置。
         * 如果在计划时间轴上启用了用户分配，则如果完成分配将导致用户被过度分配，则会显示红色的过度分配指示器。\
            有关过度分配指标的详细信息，请参阅 [分配指标](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * 没有资格接收分配的用户将变暗。
      * 展开要分配的任务或问题，单击 **分配** 字段中，开始键入要分配的用户名称，然后在下拉列表中单击该用户的名称。\
         ![schedule_task_expanded.png](assets/schedule-task-expanded-350x170.png)
   * 要推迟分配，请将您尚未准备好分配回的任何任务或问题拖回 **未分配** 的上界。



1. 单击 **进行分配** 按钮以完成任何建议的分配。\
   或\
   单击 **取消** 将所有拟派任务交还原职。

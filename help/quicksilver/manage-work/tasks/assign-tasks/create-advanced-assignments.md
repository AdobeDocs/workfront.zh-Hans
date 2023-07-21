---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 创建高级分配
description: 您可以使用高级分配管理任务或问题分配。
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 0%

---

# 创建高级分配

{{highlighted-preview}}

您可以使用高级分配管理任务或问题分配。

在进行高级分配时，您可以调整以下分配信息：

* 将用户分配给任务或问题（这可以在高级分配之外完成）。
* 调整并重新分配每个被分配人的分配小时数。
* 确定应指定为任务或问题的所有者或主要被分配人的用户。
* 指定在处理任务或问题时每个用户所履行的职责。
* <span class="preview">覆盖工作角色的记帐费率。</span>

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表进行的可用性会影响任务和问题的计划和预计日期。 有关时间表的信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Adobe Workfront中可执行高级任务的区域

本文介绍了如何在任务或问题的标题中访问高级分配。

此外，您还可以在Workfront的以下区域进行高级分配：

* 在列表中和报告中，当“工作总揽”字段显示在视图中。
* 编辑任务时，显示在“工作总揽”部分。 有关更多信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在任务或问题标题中，在任务区域中。
* 在工作负载均衡器中。 有关更多信息，请参阅 [使用工作负载均衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为任务或问题提供或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 进行高级分配

1. 转到要分配任务或问题的项目。
1. 单击 **任务** 或 **问题** 在左侧面板中，然后单击列表中的任务或问题的名称。

   >[!TIP]
   >
   >如果有两个或更多人员被分配，您可以直接在任务或问题列表中进行高级分配。 在 **指定任务** 与任务或问题位于同一行的字段，然后单击 **人员图标** 以打开“高级分配”窗口。 跳至步骤5以继续创建高级分配。\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. 单击 **分配给** 在 **指定任务** 任务或问题标题中的字段

   或

   如果任务或问题已分配，则单击分配的名称。

1. 单击 **高级**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 在 **搜索人员、角色和团队** 字段中，开始键入用户、角色或团队的名称，然后在名称出现在下拉列表中时单击该名称。

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含该特殊字符。

1. （可选）继续在中添加被分配人 **搜索人员、角色或团队** 框将多个资源添加到任务或问题。

   >[!TIP]
   >
   >* 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >* 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。
   >用户必须与至少一个工作角色关联，才能在添加时查看该角色。
   >您必须在访问级别中启用“查看联系人信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* <span class="preview">添加工作角色分配时，您可以搜索工作角色或位置。 选择系统/默认工作角色以使用分配的默认开单费率，或选择费率卡工作角色以在分配层改写费率。 有关费率卡的详细信息，请参阅 [管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
   >
   >
   >* 如果在停用用户、工作角色或团队之前分配了用户、工作角色或团队，则他们仍会分配到工作项。 在这种情况下，我们建议执行以下操作：
   >   
   >   * 将工作项重新分配给有效资源。
   >   * 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。
   >   
   >

1. 对于 **被分派人** 列中，指定以下信息：


   * **所有者**：将鼠标悬停在被分派人姓名上，然后单击 **设为主要播放器** （如果要将受分配人标记为任务或问题所有者）。 绿色复选框表示指定的用户是任务或问题的主要联系人。 Adobe Workfront将您分配给任务或问题的第一个用户或工作角色标记为所有者或主要分配。 不能将团队指定为任务或问题的主要所有者。

     >[!IMPORTANT]
     >
     >根据您的Workfront管理员或组管理员如何设置项目首选项，当您有多个用户分配到任务时，Workfront可能会使用任务所有者的时间表计算任务的时间线。 有关多个任务被分配人的信息，请参阅文章中的“将多个用户分配给任务”一节 [分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **分配** ：当任务的持续时间类型为简单时，指定每个用户或工作角色应分配给任务的小时数。 每个用户的所有分配小时数之和等于 **计划小时数** “分配”列底部的字段。 在所有其他情况下，指定您希望被分派人解决任务或问题所花费的时间（或分配）的百分比。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * 在手动修改任务的分配后，任务的已计划小时数可能会相应地更新。 有关更多信息，请参阅文章中的“管理用户分配时更新任务已计划小时数”部分 [计划小时数概述](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * 您无法手动修改问题的分配分配。
     >   * 您无法手动修改分配给任务的团队的分配。
     >   
     >

   * **被分派人的角色：** 选择用户在完成此分配时应使用的角色。  默认显示用户的主要角色。 单击“被分派人的角色”框以选择另一个角色。  在将任务或问题首先分配给角色，然后添加能够履行该角色的用户作为第二次分配时，将为能够履行已分配给任务和问题的角色的用户过滤建议用户列表。

     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   <div class="preview">

   * **位置**：如果附加到项目的费率卡使用具有工作角色的位置，则该位置来自费率卡。 无法更改位置。

   * **记帐费率**：用户的计费率来自用户或其关联工作角色的系统费率。 工作角色的记帐费率来自系统费率或费率卡（如果费率卡已附加到项目）。 现有记帐费率不显示在此字段中。 单击字段以更改此特定任务分配的记帐费率。

   </div>

   * **持续时间类型**：这仅适用于任务。 单击持续时间类型的名称，然后从下拉菜单中选择持续时间类型。 有关持续时间类型的信息，请参见 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **持续时间：** 当您具有任务的“管理”权限时，可以更新任务的此字段。

     有关更多信息，请参阅 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 批量编辑分配信息时，会出现一个类似的对话框，用于分配用户、小时、分配和任务所有者。

   * **计划小时数**：当持续时间类型为计算分配或简单时，更新已计划小时数。 因此，每个资源的分配百分比或小时数会平均分配。 当计算出的持续时间类型是“工作”或“投入比导向”时，Workfront会计算计划小时数。 有关更多信息，请参阅 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

     生产环境中的示例图像：

     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     “预览”环境中的示例图像：

     ![高级工作](assets/advanced-assignments-location-billing-rates.png)

     </div>

1. 单击&#x200B;**保存**。

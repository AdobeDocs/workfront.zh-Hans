---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 创建高级工作
description: 您可以使用“高级工作”管理任务或问题工作。
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 0%

---

# 创建高级工作

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第三季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

您可以使用“高级工作”管理任务或问题工作。

在进行高级分配时，您可以调整以下分配信息：

* 将用户分配给任务或问题（可在高级分配之外完成）。
* 调整并重新分配每个被分配人的分配小时数。
* 确定应指定为任务或问题的所有者或主要受分配人的用户。
* 指定每个用户在处理任务或问题时执行的角色。
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>在分配用户进行工作时，其根据时间表的可用性会影响任务和问题的计划和预计日期。 有关时间表的信息，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Adobe Workfront中可执行高级任务的区域

本文介绍了如何在任务或问题的标题中访问高级工作。

此外，您还可以在Workfront的以下区域进行高级分配：

* 在列表和报表中，当“工作总揽”字段显示在视图中时。
* 编辑任务时显示在“工作总揽”部分。 有关更多信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 在任务或问题标题的工作区区域中。
* 在工作负载均衡器中。 有关更多信息，请参阅 [使用工作负载均衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 进行高级工作

1. 转到要分配任务或问题的项目。
1. 单击 **任务** 或 **问题** 在左侧面板中，单击列表中的任务或问题的名称。

   >[!TIP]
   >
   >如果有两个或更多人员被分配，您可以直接在任务或问题列表中进行高级分配。 在 **指定任务** 与任务或问题位于同一行的字段，然后单击 **“人员”图标** 打开“高级分配”窗口。 跳至步骤5以继续创建高级工作。\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. 单击 **分配给** 在 **指定任务** 任务或问题标题中的字段

   或

   如果任务或问题已分配，则单击分配的名称。

1. 单击 **高级**.

   生产环境中的示例图像：
   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

   <span class="preview">“预览”环境中的示例图像：</span>
   ![单击“高级”](assets/assignments-box-in-task-header.png)

1. 在 **搜索人员、角色和团队** 字段中，开始键入用户、角色或团队的名称，然后在名称出现在下拉列表中时单击该名称。

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

1. （可选）继续在中添加被分配人 **搜索人员、角色或团队** 框将多个资源添加到任务或问题。

   >[!TIP]
   >
   >* 您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >* 添加用户分配时，请注意头像、用户的主要角色或其电子邮件地址，以区分具有相同名称的用户。
   >用户必须与至少一个工作角色关联，才能在添加时查看工作角色。
   >您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅 [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* 如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
   >   
   >   * 将工作项重新分配给活动资源。
   >   * 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. 对于 **被分派人** 列中，指定以下信息：


   * **所有者**：将鼠标悬停在被分配人的名称上并单击 **设为主要播放器** （如果要将受分配人标记为任务或问题所有者），请转至“所有者”字段。 绿色复选框表示指定用户是任务或问题的主要联系人。 Adobe Workfront将您分配给任务或问题的第一个用户或工作角色标记为“所有者”或“主要分配”。 不能将团队指定为任务或问题的主要所有者。

     >[!IMPORTANT]
     >
     >根据您的Workfront管理员或组管理员如何设置项目首选项，当您有多个用户分配到任务时，Workfront可能会使用任务所有者的时间表计算任务的时间表。 有关多个任务被分配人的信息，请参阅文章中的“将多个用户分配给任务”部分 [分配任务](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **分配** ：当任务的持续时间类型为简单时，指定每个用户或工作角色应分配给任务的小时数。 每个用户所有分配小时数的总和等于 **计划小时数** “分配”列底部的字段。 在所有其它情况下，指定您希望被分派人解决任务或问题所花费的时间（或分配）百分比。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * 在手动修改任务的分配分配后，任务的已计划小时数可能会相应地更新。 有关更多信息，请参阅文章中的“管理用户分配时更新任务已计划小时数”部分 [计划小时数概述](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * 您无法手动修改问题的分配分配。
     >   * 您无法手动修改分配给任务的团队的分配。
     >   
     >

   * **被分派人的角色：** 选择用户在完成此分配时应使用的角色。  默认情况下，将显示用户的主要角色。 单击被分配人的角色框以选择另一个角色。  在将任务或问题首先分配给角色，然后添加可以履行该角色的用户作为第二次分配时，将为可以履行已分配给任务和问题的角色的用户过滤建议用户列表。

     生产环境中的示例图像：
     ![](assets/advanced-assignments-box-select-a-role-350x243.png)

     <span class="preview">“预览”环境中的示例图像：</span>
     ![被分派人的角色](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **持续时间类型**：这仅适用于任务。 单击持续时间类型的名称，然后从下拉菜单中选择持续时间类型。 有关持续时间类型的信息，请参见 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **持续时间：** 当您具有任务的管理权限时，可以为任务更新此字段。

     有关更多信息，请参阅 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). 批量编辑分配信息时，会出现一个类似的对话框，用于分配用户、小时、分配和任务所有者。

   * **计划小时数**：当持续时间类型为计算分配或简单时，更新已计划小时数。 因此，每个资源的分配百分比或小时数会平均分配。 当持续时间类型为计算工作或投入比驱动时，Workfront会计算已计划小时数。 有关更多信息，请参阅 [任务工期和工期类型概览](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

     生产环境中的示例图像：
     ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

     <div class="preview">

     “预览”环境中的示例图像：
     ![高级工作](assets/advanced-assignments-duration-type-allocations.png)

     </div>

1. 单击&#x200B;**保存**。
